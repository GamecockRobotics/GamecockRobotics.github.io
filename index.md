---
layout: home
title: "About"
---

<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Fira Sans">
<style>
    .about-content {
        display: flex;
        flex-direction: row;
        align-items: stretch;
    }
    .main {
        max-width: 800px;
        width: 70%;
    }
    .main p, .main h1, .main h2, .main h3 {
        color: {{ site.data.theme.on_background }};
        text-align: center;
        font-family: fira sans;
    }
    .aside {
        width: 30%;
    }
    .sticky {
        position: sticky;
        top: 85px;
    }
    .sponsor {
        display: flex;
        flex-direction: row;
        width: 100%;
        align-items: center;
        justify-content: center;
    }
    .sponsor img {
        max-width: 100%;
    }
    .team-intro img {
        max-width: 100%;
    }
    .game-intro {
        width: 100%;
        font-family: fira sans;
    }
    .video {
        width: 50%;
        min-width: 240px;
        margin-top: 100px;
        padding-left: 30px;
    }
    .discord {
        text-align: center;
        align-items: center;
        font-family: fira sans;
    }
    ul {
        list-style-type: none;
    }  
    .responsive {
        max-width: 60%;
        height: auto;
        align-items: center;
        justify-content: center;
    }
    .sponsor-content {
        margin: 2px;
    }
    .sponsors {
        display: flex;
        flex-direction: column;
    }
    h1 {
        text-align: center;
    }
    .star img {
        width: 50px;
        height: 50px;
    }
    .iframe-container {
        display:flex;
        justify-content:center;
    }
    @media (max-width: 1400px) {
        .main {
            width: 100%;
            max-width: 800px;
        }
        .about-content {
        display: flex;
        flex-direction: row;
        justify-content: center;
    }
    }
</style>
<div class="about-content">
    <div class="main">
        {% include uofsc/team-intro.html %}
        {% include uofsc/game-intro.html %}
        <div class = "discord">
            <h2>Join Our Discord!</h2>
            <p>If you are interested in learning more about our club, joining our club, or just joining a community of people passionate about robotics, join our discord. Our discord has all of our important announcements, meeting times and discussions about robot designs.</p>
            <img src="/assets/socials/discord-qrcode.png" alt = "discord qr code" class = "responsive">
        </div>
        {% include uofsc/officers.html %}
        {% include uofsc/sponsors.html %}
    </div>
</div>
