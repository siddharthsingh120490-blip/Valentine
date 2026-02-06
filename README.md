# Valentine
<!DOCTYPE html>
<html>
<head>
    <title>A Special Invitation</title>
    <style>
        body { display: flex; flex-direction: column; align-items: center; justify-content: center; height: 100vh; font-family: 'Arial', sans-serif; background-color: #ffeef2; overflow: hidden; }
        h1 { color: #d63384; }
        .buttons { margin-top: 20px; }
        button { padding: 15px 30px; font-size: 18px; cursor: pointer; border-radius: 10px; border: none; margin: 10px; transition: 0.3s; }
        #yesBtn { background-color: #ff4d6d; color: white; }
        #noBtn { background-color: #888; color: white; position: absolute; }
    </style>
</head>
<body>
    <h1>Will you be my Valentine? ❤️</h1>
    <img src="https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExOHYyZzR0YXJ0Mnd4eGZ6eXN6eXN6eXN6eXN6eXN6eXN6eXN6eXN6ZSZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9cw/cLS1cfxvGOPVpf9g3y/giphy.gif" width="200">
    
    <div class="buttons">
        <button id="yesBtn" onclick="celebrate()">Yes</button>
        <button id="noBtn" onmouseover="moveButton()" onclick="moveButton()">No</button>
    </div>

    <script>
        function moveButton() {
            const x = Math.random() * (window.innerWidth - document.getElementById('noBtn').offsetWidth);
            const y = Math.random() * (window.innerHeight - document.getElementById('noBtn').offsetHeight);
            document.getElementById('noBtn').style.left = `${x}px`;
            document.getElementById('noBtn').style.top = `${y}px`;
        }
        function celebrate() {
            document.body.innerHTML = "<h1>Yay! See you on the 14th! 🥰</h1><img src='https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExbWpueWpueWpueWpueWpueWpueWpueWpueWpueWpueWpueZSZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9cw/K97pX7T5k3O2O/giphy.gif'>";
        }
    </script>
</body>
</html>
