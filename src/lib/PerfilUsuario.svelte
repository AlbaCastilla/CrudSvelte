<script>
    let name = "Jane Doe";
    let email = "janedoe@gmail.com";
    let address = "House";
    let age = "";
    let phone = "123456789";
    let profilePicture = "/fotoPerfil.png";
    let notifications = false;
</script>

<link rel="stylesheet" href="../public/css/perfilUsuario.css">
<div class="profile-container">
    <h3>{name}'s Profile</h3>
    <div class="fotoPerfil" style="background-image: url('{profilePicture}');"></div>
    <input class="input-field" type="text" placeholder="Name" bind:value={name} />
    <input class="input-field" type="email" placeholder="Email" bind:value={email} />
    <input class="input-field" type="text" placeholder="Address" bind:value={address} />
    <input class="input-field" type="text" placeholder="Phone Number" bind:value={phone} />
    <input class="input-field" type="number" placeholder="Age" bind:value={age} />
    <div class="checkbox-container">
        <label for="notifications">Enable Notifications</label>
        <input type="checkbox" bind:checked={notifications} />
    </div>
    <button class="save-btn">Save</button>
</div>
