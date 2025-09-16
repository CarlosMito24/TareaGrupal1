<template>
    <div class="container">
        <section class="card" aria-label="Formulario de inicio de sesión">
            <div class="brand" aria-label="Marca">
                <span class="brand-title">Red Social</span>
            </div>

            <h1>Inicia sesión</h1>
            <p class="helper">Inicia sesión con tu correo electrónico o usuario y tu contraseña.</p>

            <form id="loginForm" action="#" method="post" autocomplete="on">

                <label for="emailOrUser">Correo o usuario</label>
                <input type="text" id="emailOrUser" name="emailOrUser" placeholder="tú@ejemplo.com" required />

                <label for="password">Contraseña</label>
                <input type="password" id="password" name="password" placeholder="••••••••" required />

                <div style="display:flex; align-items:center; gap:6px;">
                    <input type="checkbox" id="remember" name="remember" />
                    <label for="remember" style="font-size:13px; margin:0;">Recordarme</label>
                    <a href="#" class="link" aria-label="Recuperar contraseña">¿Olvidaste tu contraseña?</a>
                </div>

                <button class="button" type="submit" aria-label="Entrar">
                    Iniciar sesión
                </button>

                <div class="footer">
                    ¿No tienes cuenta? <a href="#" class="link" aria-label="Registrarte">Crear una cuenta</a>
                </div>
            </form>
        </section>
    </div>
</template>

<script>

</script>

<style>
:root {
    --bg: #f5f6f7;
    --card: #ffffff;
    --primary: #1877f2;
    /* tono Facebook-ish */
    --text: #1f2937;
    --muted: #606770;
    --border: #dfe3e6;
    --shadow: 0 4px 14px rgba(0, 0, 0, .08);
}


html,
body {
    height: 100%;
    margin: 0;
    font-family: Inter, Roboto, Arial, sans-serif;
    background: linear-gradient(#f5f6f7, #eef2f5);
}

/* Contenedor centrado */
.container {
    min-height: 100%;
    display: grid;
    place-items: center;
    padding: 40px;
}

/* Tarjeta de login */
.card {
    width: 100%;
    max-width: 420px;
    background: var(--card);
    border: 1px solid var(--border);
    border-radius: 12px;
    padding: 28px 28px 20px;
    box-shadow: var(--shadow);
}

.brand {
    display: flex;
    align-items: center;
    gap: 12px;
    margin-bottom: 18px;
}

.brand-logo {
    width: 40px;
    height: 40px;
    border-radius: 8px;
    background: linear-gradient(135deg, #1877f2 0%, #4cc9f0 100%);
    display: inline-block;
}

.brand-title {
    font-weight: 700;
    font-size: 20px;
    color: #1e1e1e;
}

h1 {
    font-size: 22px;
    margin: 10px 0 6px;
    color: #1e1e1e;
}

p.helper {
    color: var(--muted);
    font-size: 14px;
    margin: 6px 0 18px;
}

/* Formulario */
form {
    display: grid;
    gap: 12px;
}

label {
    font-size: 12px;
    font-weight: 600;
    color: #333;
}

input[type="text"],
input[type="email"],
input[type="password"] {
    width: 100%;
    padding: 12px 14px;
    border: 1px solid var(--border);
    border-radius: 8px;
    font-size: 14px;
    background: #fff;
}

input:focus {
    outline: none;
    border-color: var(--primary);
    box-shadow: 0 0 0 3px rgba(24, 119, 242, .15);
}

.row {
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 12px;
}

.button {
    width: 100%;
    padding: 12px 14px;
    border: none;
    border-radius: 8px;
    background: var(--primary);
    color: white;
    font-weight: 700;
    cursor: pointer;
    font-size: 15px;
}

.button:disabled {
    opacity: .6;
    cursor: not-allowed;
}

.link {
    font-size: 13px;
    color: var(--primary);
    text-decoration: none;
    font-weight: 600;
}

.footer {
    text-align: center;
    font-size: 12px;
    color: var(--muted);
}
</style>