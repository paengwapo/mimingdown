[deepseek_html_20251024_723719.html](https://github.com/user-attachments/files/23135131/deepseek_html_20251024_723719.html)
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Para sa aking Shrekina</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Arial Rounded MT Bold', 'Arial', sans-serif;
        }
        
        body {
            background: linear-gradient(135deg, #ffc8dd, #ffafcc);
            min-height: 100vh;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            padding: 20px;
            color: #590d82;
        }
        
        .container {
            max-width: 600px;
            width: 100%;
            background-color: rgba(255, 255, 255, 0.9);
            border-radius: 20px;
            padding: 30px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
            text-align: center;
            margin-bottom: 20px;
        }
        
        h1 {
            font-size: 2.2rem;
            margin-bottom: 20px;
            color: #ff006e;
            text-shadow: 2px 2px 0px #ffb5e8;
        }
        
        .button-container {
            margin: 25px 0;
        }
        
        .cute-button {
            background: linear-gradient(to right, #ff5e9a, #ff85a1);
            border: none;
            border-radius: 50px;
            padding: 15px 30px;
            font-size: 1.2rem;
            color: white;
            cursor: pointer;
            box-shadow: 0 5px 15px rgba(255, 94, 154, 0.4);
            transition: all 0.3s ease;
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 10px;
            margin: 0 auto;
        }
        
        .cute-button:hover {
            transform: translateY(-3px);
            box-shadow: 0 8px 20px rgba(255, 94, 154, 0.6);
        }
        
        .cute-button:active {
            transform: translateY(1px);
        }
        
        .message {
            display: none;
            background-color: #f8f9fa;
            border-radius: 15px;
            padding: 25px;
            margin-top: 25px;
            text-align: left;
            line-height: 1.6;
            font-size: 1rem;
            border-left: 5px solid #ff5e9a;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
        }
        
        .cat-emoji {
            font-size: 1.5rem;
        }
        
        .footer {
            margin-top: 20px;
            font-size: 0.9rem;
            color: #6a0572;
            text-align: center;
        }
        
        /* Mobile-specific styles */
        @media (max-width: 600px) {
            h1 {
                font-size: 1.8rem;
            }
            
            .container {
                padding: 20px;
            }
            
            .cute-button {
                padding: 12px 25px;
                font-size: 1.1rem;
            }
            
            .message {
                padding: 20px;
                font-size: 0.95rem;
            }
        }
        
        @media (max-width: 400px) {
            h1 {
                font-size: 1.5rem;
            }
            
            .cute-button {
                padding: 10px 20px;
                font-size: 1rem;
            }
            
            .message {
                padding: 15px;
                font-size: 0.9rem;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Para sa aking Shrekina</h1>
        
        <div class="button-container">
            <button class="cute-button" id="messageButton">
                <span class="cat-emoji">😻🐱</span>
                Press me kikinn
                <span class="cat-emoji">🐾💖</span>
            </button>
        </div>
        
        <div class="message" id="hiddenMessage">
            One thing I love most about you is that you never fail to cheer me up, imong mga horny nga kabuang, okay fine, atong mga chika pud abt ni nikol sd 😭 but most times, you message and listen to me. When I ignored everyone and from you, I still felt your love in the words you uttered and the things you did when you welcomed me back:)) You never made me feel as if I'm something to be fixed or patched up. You just let me be. I feel like I can exist and be enough with doing just so. Point is, you show up🥹 for us and pls know that you don't have to worry about finding someone like that. Me and Mege will be that person for you 🫶 ALSO diay one thing I learned about love with you is that it's polite. It's polite and it comes to find me. It knocks and waits for me to welcome it in my home. My shrekina thank you for not opening my door by force. Thank you for knocking. Thank you for waiting for me to open the door for you myself.
        </div>
    </div>
    
    <div class="footer">
        Made with love for my Shrekina 💚
    </div>

    <script>
        document.getElementById('messageButton').addEventListener('click', function() {
            const message = document.getElementById('hiddenMessage');
            message.style.display = 'block';
            
            // Add a little animation
            message.style.opacity = '0';
            message.style.transform = 'translateY(20px)';
            
            let opacity = 0;
            let position = 20;
            const fadeIn = setInterval(() => {
                opacity += 0.05;
                position -= 1;
                message.style.opacity = opacity;
                message.style.transform = `translateY(${position}px)`;
                
                if (opacity >= 1) {
                    clearInterval(fadeIn);
                    message.style.transform = 'translateY(0)';
                }
            }, 30);
            
            // Change button text after click
            this.innerHTML = '<span class="cat-emoji">😽💕</span> Thank you for being you! <span class="cat-emoji">💖🐱</span>';
            this.style.background = 'linear-gradient(to right, #a166ab, #cdb4db)';
        });
    </script>
</body>
</html>
