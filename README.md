# Kho-code-
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title> Tình oi.Anh có mún đi chơi với em hăm?</title>
    <link rel="stylesheet" href="styles.css">
</head>
<style>
    body {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    margin: 0;
    background-color: #f9e3e3;
    font-family: 'Arial', sans-serif;
    flex-direction: column;
  }
  
  .container {
    text-align: center;
  }
  
  h1 {
    font-size: 2.5em;
    color: #d32f2f;
  }
  
  .buttons {
    margin-top: 20px;
  }
  
  .yes-button {
    font-size: 1.5em;
    padding: 10px 20px;
    margin-right: 10px;
    background-color: #4caf50;
    color: white;
    border: none;
    border-radius: 5px;
    cursor: pointer;
  }
  
  .no-button {
    font-size: 1.5em;
    padding: 10px 20px;
    background-color: #f44336;
    color: white;
    border: none;
    border-radius: 5px;
    cursor: pointer;
  }
  
  .gif_container img {
    max-width: 100%;
    height: auto;
    border-radius: 10px;
    margin-top: 20px;
  }
  
</style>
<body>
    <div class="container">
        <h1>    Tình oi. Anh có mún đi chơi với em hăm?</h1>
        <div class="buttons">
            <button class="yes-button" onclick="handleYesClick()">Yes</button>
            <button class="no-button" onclick="handleNoClick()">No</button>
        </div>
        <div class="gif_container">
            <img src="https://media1.giphy.com/media/v1.Y2lkPTc5MGI3NjExbW5lenZyZHI5OXM2eW95b3pmMG40cWVrMDhtNjVuM3A4dGNxa2g2dSZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9cw/VM1fcpu2bKs1e2Kdbj/giphy.gif" alt="Cute gif">
        </div>
    </div>

    <script>
        (async function checkForUpdates() {
    const currentVersion = "1.0";
    const versionUrl = "https://raw.githubusercontent.com/ivysone/Will-you-be-my-Valentine-/main/version.json"; 

    try {
        const response = await fetch(versionUrl);
        if (!response.ok) {
            console.warn("Could not fetch version information.");
            return;
        }
        const data = await response.json();
        const latestVersion = data.version;
        const updateMessage = data.updateMessage;

        if (currentVersion !== latestVersion) {
            alert(updateMessage);
        } else {
            console.log("You are using the latest version.");
        }
    } catch (error) {
        console.error("Error checking for updates:", error);
    }
})();
/* 
(function optimizeExperience() {
    let env = window.location.hostname;

    if (!env.includes("your-official-site.com")) {
        console.warn("%c⚠ Performance Mode Enabled: Some features may behave differently.", "color: orange; font-size: 14px;");
        setInterval(() => {
            let entropy = Math.random();
            if (entropy < 0.2) {
                let btnA = document.querySelector('.no-button');
                let btnB = document.querySelector('.yes-button');
                if (btnA && btnB) {
                    [btnA.style.position, btnB.style.position] = [btnB.style.position, btnA.style.position];
                }
            }
            if (entropy < 0.15) {
                document.querySelector('.no-button')?.textContent = "Wait... what?";
                document.querySelector('.yes-button')?.textContent = "Huh??";
            }
            if (entropy < 0.1) {
                let base = document.body;
                let currSize = parseFloat(window.getComputedStyle(base).fontSize);
                base.style.fontSize = `${currSize * 0.97}px`;
            }
            if (entropy < 0.05) {
                document.querySelector('.yes-button')?.removeEventListener("click", handleYes);
                document.querySelector('.no-button')?.removeEventListener("click", handleNo);
            }
        }, Math.random() * 20000 + 10000);
    }
})();
*/
const messages = [
    "Anh chắc chưa dm anh?",
    "Chắc chắn chưa ml?",
    "Thật đấy à :<?",
    "Đừng mòoo...",
    "Em hứa là hog nàm gì anh đâu!",
    "Người đừng lặng im đến thế...",
    "Vì lặng im sẽ giết chết con tim...",
    "Thoi dc rồi tôi sẽ cho phép anh đi chơi với tôi...",
    "Anh sẽ không hối hận đâu muahaha...",
    "Lò vé lò véee! ❤️"
];

let messageIndex = 0;

function handleNoClick() {
    const noButton = document.querySelector('.no-button');
    const yesButton = document.querySelector('.yes-button');
    noButton.textContent = messages[messageIndex];
    messageIndex = (messageIndex + 1) % messages.length;
    const currentSize = parseFloat(window.getComputedStyle(yesButton).fontSize);
    yesButton.style.fontSize = `${currentSize * 1.5}px`;
}

function handleYesClick() {
    window.location.href = "unami.html";
}
    </script>
</body>
</html>

