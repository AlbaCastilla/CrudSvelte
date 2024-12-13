<script>
    let email = "";
    let password = "";
</script>
<link rel="stylesheet" href="../public/css/loginUsuario.css">

<div class="registration-container">
    <span class="back-arrow">&#x2190;</span> 
    <h2>Welcome to TeachEase</h2>
    <p>Welcome back! Sign in using your email to continue</p>

    <input class="input-field" type="email" placeholder="Email" bind:value={email} />
    <input class="input-field" type="password" placeholder="Password" bind:value={password} />
    
    <button class="login-btn">Sign in</button>
</div>
