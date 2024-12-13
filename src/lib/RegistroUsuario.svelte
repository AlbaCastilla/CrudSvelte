<script>
    let username = "";
    let email = "";
    let password = "";
    let confirmPassword = "";

    function register() {
        // Crear un array con los datos
        const userData = {
            username,
            email,
            password,
            confirmPassword
        };

        // Mostrar el array en la consola
        console.log(userData);
    }
</script>
<link rel="stylesheet" href="../public/css/registroUsuario.css">

<div class="registration-container">
    <span class="back-arrow">&#x2190;</span>
    <h2>Sign up with Email</h2>
    <p>Start organizing your freelancing career as a private tutor and sign in using your email!</p>
    
    <input class="input-field" type="text" placeholder="Username" bind:value={username} />
    <input class="input-field" type="email" placeholder="Email" bind:value={email} />
    <input class="input-field" type="password" placeholder="Password" bind:value={password} />
    <input class="input-field" type="password" placeholder="Confirm Password" bind:value={confirmPassword} />
    
    <button class="register-btn" on:click={register}>Register account</button>
</div>
