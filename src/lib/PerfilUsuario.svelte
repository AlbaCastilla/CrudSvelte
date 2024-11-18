<script>
    let name = "Jane Doe";
    let email = "janedoe@gmail.com";
    let address = "House";
    let age = "20";
    let phone = "123456789";
    let profilePicture = "/fotoPerfil.png";
</script>

<style>
    .profile-container {
        display: flex;
        flex-direction: column;
        align-items: center;
        padding: 4vh;
        max-width: 90vw; 
        margin: 0 auto;
        border: 0.2vh solid #e0e0e0;
        border-radius: 1.5vh;
        background-color: #f7f7f7;
        box-shadow: 0 0.8vh 2vh rgba(0, 0, 0, 0.1);
        font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        transition: transform 0.3s ease;
        text-align: center;
    }

    .profile-container:hover {
        transform: scale(1.02);
        box-shadow: 0 1vh 2.5vh rgba(0, 0, 0, 0.15);
    }

    .profile-container h3 {
        font-size: 3vh;
        margin-bottom: 2vh;
        color: #333;
        font-weight: 600;
    }

    .fotoPerfil {
        width: 15vh;
        height: 15vh;
        background-size: cover;
        background-position: center;
        border-radius: 50%;
        margin-bottom: 2vh;
        border: 0.6vh solid rgb(227, 69, 122);
        box-shadow: 0 0.6vh 1.2vh rgba(0, 0, 0, 0.1);
        transition: transform 0.2s ease, box-shadow 0.3s ease;
    }

    .fotoPerfil:hover {
        transform: scale(1.1);
        box-shadow: 0 1vh 2vh rgba(0, 0, 0, 0.2);
    }

    .input-field {
        width: 100%;
        max-width: 60vw;
        padding: 1.2vh;
        margin: 1vh 0;
        border-radius: 0.6vh;
        border: 0.1vh solid #ddd;
        background-color: #fff;
        font-size: 2vh;
    }

    .input-field:focus {
        border-color: rgb(227, 69, 122);
        outline: none;
    }

    .save-btn {
        background-color: rgb(227, 69, 122);
        color: white;
        border: none;
        padding: 1.2vh 3vw;
        width: 40vw;
        border-radius: 0.8vh;
        font-size: 2vh;
        cursor: pointer;
        margin-top: 1.5vh;
        transition: background-color 0.3s ease, transform 0.2s ease;
    }

    .save-btn:hover {
        background-color: rgb(205, 21, 82);
        transform: scale(1.05);
        outline: none;
    }

    .save-btn:active {
        transform: scale(1);
        outline: none;
    }

    .save-btn:focus {
    outline: none;
    background-color: rgb(205, 21, 82);
    transform: scale(1);
    }
</style>

<div class="profile-container">
    <h3>{name}'s Profile</h3>
    <div class="fotoPerfil" style="background-image: url('{profilePicture}');"></div>
    <input class="input-field" type="text" placeholder="Name" bind:value={name} />
    <input class="input-field" type="email" placeholder="Email" bind:value={email} />
    <input class="input-field" type="text" placeholder="Address" bind:value={address} />
    <input class="input-field" type="text" placeholder="Phone Number" bind:value={phone} />
    <input class="input-field" type="number" placeholder="Age" bind:value={age} />
    <button class="save-btn">Save</button>
</div>
