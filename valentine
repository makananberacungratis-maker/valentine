<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>A Question For You</title>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&display=swap" rel="stylesheet">

<style>
    body {
        margin: 0;
        height: 100vh;
        font-family: 'Poppins', sans-serif;
        display: flex;
        justify-content: center;
        align-items: center;
        background: linear-gradient(135deg, #ffe0ec, #fff7d6);
        overflow: hidden;
    }

    .card {
        background: white;
        padding: 40px 50px;
        border-radius: 20px;
        text-align: center;
        box-shadow: 0 20px 40px rgba(0,0,0,0.15);
        animation: pop 0.6s ease;
    }

    @keyframes pop {
        from { transform: scale(0.8); opacity: 0; }
        to { transform: scale(1); opacity: 1; }
    }

    h1 {
        font-weight: 600;
        font-size: 2rem;
        margin-bottom: 35px;
    }

    .buttons {
        position: relative;
        height: 80px;
    }

    button {
        padding: 14px 32px;
        font-size: 1rem;
        border-radius: 12px;
        border: none;
        cursor: pointer;
        transition: 0.2s ease;
    }

    #yes {
        background: #ff4d88;
        color: white;
        box-shadow: 0 10px 20px rgba(255,77,136,0.4);
    }

    #yes:hover {
        transform: scale(1.05);
    }

    #no {
        background: #eee;
        color: #444;
        position: absolute;
        left: 140px;
    }

    .heart {
        position: fixed;
        font-size: 20px;
        animation: float 3s linear forwards;
    }

    @keyframes float {
        from { transform: translateY(0); opacity: 1; }
        to { transform: translateY(-150px); opacity: 0; }
    }
</style>
</head>

<body>

<div class="card" id="card">
    <h1>Will you be my valentine? 💌</h1>
    <div class="buttons">
        <button id="yes">Yes 💖</button>
        <button id="no">No 🙄</button>
    </div>
</div>

<script>
    const noBtn = document.getElementById("no");
    const yesBtn = document.getElementById("yes");

    noBtn.addEventListener("mouseover", () => {
        const x = Math.random() * 250 - 120;
        const y = Math.random() * 120 - 60;
        noBtn.style.transform = `translate(${x}px, ${y}px)`;
    });

    yesBtn.addEventListener("click", () => {
        document.getElementById("card").innerHTML = "<h1>YAYYYY 💕🥰<br>I knew it!</h1>";
        setInterval(createHeart, 200);
    });

    function createHeart() {
        const heart = document.createElement("div");
        heart.className = "heart";
        heart.innerHTML = "💖";
        heart.style.left = Math.random() * window.innerWidth + "px";
        heart.style.bottom = "0px";
        document.body.appendChild(heart);

        setTimeout(() => heart.remove(), 3000);
    }
</script>

</body>
</html>
