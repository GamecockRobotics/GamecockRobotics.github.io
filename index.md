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
    <div class = "container">
        <div class = "left-div">
            <h1 style="text-align: center">VEX Robotics: Spin Up</h1>
                <p>
                    Vex is a head to head competition where teams compete with two robots to score more points than the other team. Teams design, build, program and drive the robots. Each year a different challenge is presented.
                </p>
                <p>
                    Gamecock Robotics was founded in 2021 as the robotics team for the University of South Carolina. The team has 11 members and 1 faculty advisor.
                </p> 
                <div class = "iframe-container">
                <iframe width="680" height="383" src="https://www.youtube.com/embed/wIZgvVDZc2Y" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
                </div>
                <h1 style = "text-align: center">Join Our Discord!</h1>
                        <p>If you are interested in learning more about our club, joining our club, or just joining a community of people passionate about robotics, join our discord. Our discord has all of our important announcements, meeting times and discussions about robot designs.</p>
                        <img src="/assets/socials/discord-qrcode.png" alt = "discord qr code" class = "responsive">
        </div>
        <div class = "right-div">
                <a class="twitter-timeline" data-lang="en" data-width="750" data-height="1270" data-theme="light" href="https://twitter.com/GamecockRobotix?ref_src=twsrc%5Etfw">Tweets by GamecockRobotix</a> 
                <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script> 
        </div>
    </div>
</div>
