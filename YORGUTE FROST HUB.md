<!DOCTYPE html>
<html lang="pt-br">
<head>
<meta charset="UTF-8">
<title>YORGUTE FROST HUB SCRIPT</title>

<style>
body {
    margin: 0;
    background: #0b0b0f;
    font-family: Arial;
    color: white;
}

.container {
    width: 400px;
    margin: 50px auto;
    background: #12121a;
    border-radius: 12px;
    box-shadow: 0 0 25px #6a00ff;
    overflow: hidden;
}

.header {
    background: #1a1a25;
    padding: 15px;
    text-align: center;
    font-size: 18px;
    color: #b388ff;
}

.tabs {
    display: flex;
    background: #151520;
}

.tab {
    flex: 1;
    padding: 10px;
    text-align: center;
    cursor: pointer;
    transition: 0.3s;
}

.tab:hover {
    background: #2a2a40;
}

.tab.active {
    background: #6a00ff;
}

.content {
    padding: 20px;
    display: none;
}

.content.active {
    display: block;
}

.button {
    width: 100%;
    padding: 10px;
    margin-top: 10px;
    border: none;
    border-radius: 6px;
    background: #6a00ff;
    color: white;
    cursor: pointer;
}

.button:hover {
    background: #8e3cff;
}
</style>
</head>

<body>

<div class="container">
    <div class="header">YORGUTE FROST HUB SCRIPT</div>

    <div class="tabs">
        <div class="tab active" onclick="openTab(0)">Visual</div>
        <div class="tab" onclick="openTab(1)">Movimento</div>
        <div class="tab" onclick="openTab(2)">Extras</div>
    </div>

    <div class="content active">
        <button class="button">ESP Player</button>
        <button class="button">ESP Name</button>
        <button class="button">ESP Caixa</button>
        <button class="button">ESP Linha</button>
    </div>

    <div class="content">
        <button class="button">Speed</button>
        <button class="button">Fly</button>
        <button class="button">Teleporte</button>
    </div>

    <div class="content">
        <button class="button">Aimbot</button>
        <button class="button">FOV Circle</button>
    </div>
</div>

<script>
function openTab(index) {
    let tabs = document.querySelectorAll(".tab");
    let contents = document.querySelectorAll(".content");

    tabs.forEach(t => t.classList.remove("active"));
    contents.forEach(c => c.classList.remove("active"));

    tabs[index].classList.add("active");
    contents[index].classList.add("active");
}
</script>

</body>
</html>
