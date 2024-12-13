<script>
    let username = "";
    let email = "";
    let password = "";
    let confirmPassword = "";
    let agreeToTerms = false;
</script>

<style>
    .registration-container {
        display: flex;
        flex-direction: column;
        align-items: center;
        padding: 4vh;
        max-width: 90vw;
        margin: 0 auto;
        border: 0.2vh solid #e0e0e0;
        border-radius: 1.5vh;
        background-color: #E7EDF0;
        box-shadow: 0 0.8vh 2vh rgba(0, 0, 0, 0.1);
        font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        transition: transform 0.3s ease;
        text-align: center;
    }

    .registration-container:hover {
        transform: scale(1.02);
        box-shadow: 0 1vh 2.5vh rgba(0, 0, 0, 0.15);
    }

    .registration-container h3 {
        font-size: 3vh;
        margin-bottom: 2vh;
        color: #000;
        font-weight: 600;
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
        border-color: #577A8E;
        outline: none;
    }

    .checkbox-container {
        display: flex;
        align-items: center;
        justify-content: space-between;
        margin-top: 1.5vh;
        margin-bottom: 1.5vh;
        font-size: 2vh;
        color: #000;
        width: 100%;
        max-width: 60vw;
    }

    .checkbox-container input {
        margin-left: 1vh;
    }

    .checkbox-container label {
        margin-right: auto;
        transition: color 0.3s ease;
    }

    .checkbox-container input:checked + label {
        color: #577A8E;
    }

    .register-btn {
        background-color: #577A8E;
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

    .register-btn:hover {
        background-color: #415a68;
        transform: scale(1.05);
        outline: none;
    }

    .register-btn:active {
        transform: scale(1);
        outline: none;
    }

    .register-btn:focus {
        outline: none;
        background-color: #415a68;
        transform: scale(1);
    }
</style>

<div class="registration-container">
    <h3>Register</h3>
    <input class="input-field" type="text" placeholder="Username" bind:value={username} />
    <input class="input-field" type="email" placeholder="Email" bind:value={email} />
    <input class="input-field" type="password" placeholder="Password" bind:value={password} />
    <input class="input-field" type="password" placeholder="Confirm Password" bind:value={confirmPassword} />
    <div class="checkbox-container">
        <label for="terms">I agree to the terms and conditions</label>
        <input type="checkbox" id="terms" bind:checked={agreeToTerms} />
    </div>
    <button class="register-btn">Register</button>
</div>
