---
layout: home
title: "About"
---
<div id="about-page">
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Fira Sans">
    <style>
        .about-content {
            display: flex;
            flex-direction: row;
            align-items: stretch;
        }
        .main {
            width: 70%;
        }
        .main p, .main h1, .main h2, .main h3 {
            color: {{ site.data.theme.on_background }};
        }
        .sidebar {
            width: 75%;
            display: block;
            z-index: -1;
        }
        .sticky {
            position: sticky;
            top: 85px;
        }
        .row {
            display: flex;
            flex-direction: row;
        }
        .row .text {
            width: 100%;
            margin: 20px;
            font-family: fira sans;
        }
        .row .video {
            width: 50%;
            min-width: 240px;
            margin-top: 100px;
            padding-left: 30px;
        }
        .twitter {
            padding-bottom: 40px;
        }
        .discord {
            text-align:center;
            align-items: center;
            scale: 80%;
            font-family: fira sans;
            padding-left: 50px;
        }
        ul {
            list-style-type: none;
        }
        #my{
        zoom: 90%;
        }
        .container {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
            width: 100%;
            max-width: 1500px;
            margin: 0 15px;
            overflow: hidden;
            flex-direction: row;
            padding-bottom: 50px;
        }            
        .left-div{
            width: 48%;
            overflow: auto;
            padding 10px;
        }
        .right-div{
            width: 48%;
            overflow: auto;
            padding 10px;
        }
        .responsive {
            max-width: 60%;
            height: auto;
            align-items: center;
            justify-content: center;
        }
    @media (max-width: 1000px) {
        .left-div, .right-div {
            width: 100%;
            height: auto;
            margin: 10px 0;
        }
    }
</style>
    <div class="about-content">
        <div class="main">
            <div class="row">
                <div class="text">
                    <h1 style="text-align: center">VEX Robotics: Over Under</h1>
                    <p>
                        Every year the RECF holds robotics competitions using the VEX ecosystem. Gamecock Robotics competes in the category "VEX U". VEX U is for University teams and allows for teams to use advanced materials and building techniques such as CNC milling and 3D printing. This years game is named "Over Under"
                    </p>
                    <p>
                        Gamecock Robotics was founded in 2021 as the robotics team for the University of South Carolina. The team has 11 members and 1 faculty advisor.
                    </p> 
                    <div class = "iframe-container">
                    <iframe width="560" height="315" src="https://www.youtube.com/embed/dvDqEI7qO34?si=UV_fQya-GOKbylQW" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
                    </div>
                </div>
            </div>
        <!-- The thing -->
        <div class = "discord">
                    <h2>Join Our Discord!</h2>
                    <p>If you are interested in learning more about our club, joining our club, or just joining a community of people passionate about robotics, join our discord. Our discord has all of our important announcements, meeting times and discussions about robot designs.</p>
                    <img src="/assets/socials/discord-qrcode.png" alt = "discord qr code" class = "responsive">
        </div>
        </div>
    </div>
</div>
