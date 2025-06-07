# -dom-part-one-
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <title>Box Layout</title>
</head>

<body>
    <h2>Let's Develop It</h2>
    <div id="container">
        <div>1</div>
        <div>2</div>
        <div>3</div>
        <div>4</div>
    </div>

    <script src="script.js"></script>
</body>
<script src="n.js"></script>

</html>

# n.js
const container = document.getElementById("container");
const divs = container.querySelectorAll("div");

// Стили контейнера
container.style.display = "flex";
container.style.flexWrap = "wrap";
container.style.justifyContent = "center";
container.style.gap = "10px";
container.style.width = "680px";
container.style.marginTop = "20px";

// Применяем стили к каждому div
divs.forEach((div, index) => {
    div.style.height = "100px";
    div.style.width = index < 3 ? "200px" : "640px"; // нижний шире
    div.style.fontSize = "30px";
    div.style.backgroundColor = "#888";
    div.style.border = "15px solid rgb(54, 52, 52)";
    div.style.display = "flex";
    div.style.justifyContent = "center";
    div.style.alignItems = "center";
    div.style.borderRadius = "10px";
    div.style.boxSizing = "border-box";
});
