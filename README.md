<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>mensaje.exe</title>

<style>
* {
    box-sizing: border-box;
}

body {
    margin: 0;
    min-height: 100vh;
    background: #050505;
    color: #00ff88;
    font-family: "Courier New", monospace;
    display: flex;
    align-items: center;
    justify-content: center;
}

.terminal {
    width: 90%;
    max-width: 850px;
    min-height: 500px;
    padding: 30px;
    border: 1px solid #00ff88;
    box-shadow: 0 0 30px rgba(0,255,136,.2);
    background: #000;
}

.top {
    color: #777;
    margin-bottom: 25px;
}

.line {
    margin: 14px 0;
    opacity: 0;
    animation: aparecer .7s forwards;
}

.line:nth-child(2) { animation-delay: .6s; }
.line:nth-child(3) { animation-delay: 1.2s; }
.line:nth-child(4) { animation-delay: 1.8s; }
.line:nth-child(5) { animation-delay: 2.4s; }

.mensaje {
    opacity: 0;
    text-align: center;
    margin-top: 80px;
    animation: revelar 1.5s 3.3s forwards;
}

.mensaje h1 {
    font-size: clamp(40px, 9vw, 85px);
    margin: 0;
    text-shadow: 0 0 20px #00ff88;
    letter-spacing: 5px;
}

.mensaje p {
    color: #b7ffd9;
    font-size: 20px;
}

.cursor {
    display: inline-block;
    width: 10px;
    height: 20px;
    background: #00ff88;
    animation: parpadear .8s infinite;
}

@keyframes aparecer {
    to { opacity: 1; }
}

@keyframes revelar {
    to { opacity: 1; }
}

@keyframes parpadear {
    50% { opacity: 0; }
}
</style>
</head>

<body>

<div class="terminal">

    <div class="top">
        MARS_OS // private_message.exe
    </div>

    <div class="line">
        > iniciando sistema...
    </div>

    <div class="line">
        > buscando destinatario: MARS
    </div>

    <div class="line">
        > verificando sentimientos...
    </div>

    <div class="line">
        > resultado: 100% reales
    </div>

    <div class="line">
        > ejecutando mensaje<span class="cursor"></span>
    </div>

    <div class="mensaje">
        <h1>TE AMO, MARS</h1>

        <p>proceso completado ♡</p>

        <p>
            y esta historia todavía tiene mucho por continuar...
        </p>
    </div>

</div>

</body>
</html>
