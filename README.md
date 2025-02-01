# Dabapath
Website for dabapath
html<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Team DabaPath</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <div class="container">
        <h1><span class="team">Team</span> <span class="dabapath">DabaPath</span></h1>
        <button class="create-account">CREATE ACCOUNT</button>
        
        <h2>WHAT WE OFFER</h2>
        
        <div class="services">
            <button class="service">LANDING PAGE</button>
            <button class="service">CMS</button>
            <button class="service">UI/UX DESIGN</button>
            <button class="service">E-COMMERCE</button>
        </div>

        <div class="footer">
            <p>@REALLYGREATSITE</p>
            <p>123-456-7890</p>
        </div>
    </div>
</body>
</html>
css@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;700&display=swap');

body {
    margin: 0;
    padding: 0;
    font-family: 'Poppins', sans-serif;
    background: url('https://source.unsplash.com/1600x900/?chessboard') no-repeat center center/cover;
    color: white;
    text-align: center;
}

.container {
    padding: 50px;
}

h1 {
    font-size: 36px;
}

.team {
    font-weight: 300;
}

.dabapath {
    font-weight: 700;
    color: #F4A623;
}

.create-account {
    background: white;
    border: none;
    padding: 10px 20px;
    font-size: 14px;
    cursor: pointer;
    margin: 20px;
    font-weight: bold;
}

h2 {
    color: #F4A623;
    margin-top: 40px;
}

.services {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 15px;
    margin-top: 20px;
}

.service {
    background: white;
    color: black;
    padding: 10px 20px;
    border: none;
    font-weight: bold;
    border-radius: 5px;
    box-shadow: 0 4px 8px rgba(0, 255, 170, 0.5);
    cursor: pointer;
}

.footer {
    margin-top: 50px;
    font-size: 14px;
    color: #F4A623;
}
jsdocument.querySelectorAll('.service').forEach(button => {
    button.addEventListener('click', () => {
        alert(`You clicked on ${button.textContent}`);
    });
});
