<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Karma Tsukino</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            font-family: Arial, sans-serif;
            background-image: url('https://cdn.discordapp.com/attachments/1196281703421968487/1279132004805251295/JSJFJSDJSJFJS.png?ex=66d35403&is=66d20283&hm=6842cd57a5bedfb73522673459c0bec2335dd053690b38521c557c597378cc78&');
            background-size: cover;
            background-position: center;
            color: white;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            text-align: center;
            transition: all 0.5s ease;
        }

        .container {
            background: rgba(0, 0, 0, 0.7);
            padding: 20px;
            border-radius: 10px;
            width: 450px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.3);
            display: grid;
            grid-template-areas:
                "top-left top-right"
                "center center"
                "bottom-left bottom-right";
            grid-gap: 10px;
        }

        .profile-pic {
            width: 100px;
            height: 100px;
            border-radius: 50%;
            border: 3px solid white;
            margin: 0 auto;
            background-image: url('https://media.discordapp.net/attachments/1196281703421968487/1278920908450299934/illustration-of-boy-profile-anime-style-black-silhouette-isolated-on-white-background-free-vector.jpg?ex=66d33829&is=66d1e6a9&hm=c81b7bf4e9e0f81031d1f72d5213b33ce37816c58b981b8e5e051f281f1d6af3&=&format=webp&width=421&height=421');
            background-size: cover;
            background-position: center;
            cursor: pointer;
            grid-area: center;
        }

        .name {
            font-size: 24px;
            font-weight: bold;
            background: linear-gradient(45deg, hotpink, purple, red);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            margin-bottom: 15px;
            grid-area: center;
        }

        .bio {
            font-size: 16px;
            line-height: 1.5;
            grid-area: top-left;
            text-align: left;
        }

        .button-container {
            display: flex;
            flex-direction: column;
            gap: 6px;
        }

        .button {
            background-color: hotpink;
            color: white;
            padding: 6px;
            border: none;
            border-radius: 5px;
            text-decoration: none;
            font-weight: bold;
            font-size: 12px;
            transition: background-color 0.3s;
        }

        .button:hover {
            background-color: purple;
        }

        .top-left {
            grid-area: top-left;
            text-align: left;
        }

        .top-right {
            grid-area: top-right;
        }

        .bottom-left {
            grid-area: bottom-left;
        }

        .bottom-right {
            grid-area: bottom-right;
        }

        .secret-container {
            display: none;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: black;
            color: white;
        }

        .secret-box {
            background: black;
            border: 2px solid white;
            padding: 20px;
            text-align: center;
            font-size: 24px;
            color: white;
            cursor: pointer;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="top-left">
            <div class="bio">
                <p>Hello! I'm Karma Tsukino, the Founder of A.O.O. I am a Developer, gamer, content creator, and music producer. I love exploring new things and sharing my journey with the world. Stay tuned for more!</p>
            </div>
        </div>
        <div class="top-right">
            <div class="button-container">
                <a href="https://therealcorruption.github.io/A.O.O.-WEBPAGE/" class="button">A.O.O. Main Page</a>
                <a href="https://scratch.mit.edu/users/coolcats153122/" class="button">Scratch</a>
                <a href="https://www.roblox.com/users/4490451884/profile" class="button">Roblox</a>
                <a href="https://www.youtube.com/" class="button">YouTube</a>
            </div>
        </div>
        <div class="center">
            <div class="profile-pic" onclick="revealSecret()"></div>
            <div class="name">Karma Tsukino</div>
        </div>
        <div class="bottom-left">
            <!-- Extra space for future content -->
        </div>
        <div class="bottom-right">
            <div class="button-container">
                <a href="#" class="button">Discord Server 1</a>
                <a href="#" class="button">Discord Server 2</a>
                <!-- Add more buttons as needed -->
            </div>
        </div>
    </div>
    <div class="secret-container" id="secret-container">
        <a href="https://therealcorruption.github.io/MenuPage/" class="secret-box">Tape-1</a>
    </div>

    <script>
        function revealSecret() {
            document.body.style.backgroundColor = 'black';
            document.body.style.backgroundImage = 'none';  /* Remove the background image */
            document.querySelector('.container').style.display = 'none';
            document.getElementById('secret-container').style.display = 'flex';
        }
    </script>
</body>
</html>
