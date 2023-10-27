---
layout: home
title: "About"
---

<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Fira Sans">
<style>
    .about-content {
        display: flex;
        flex-direction: row;
        justify-content: center;
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
    .buffer {
        width: 40px;
    }
    .aside {
    }
    .sticky {
        position: sticky;
        top: 120px;
        margin-top: 60px;
        background-color: {{ site.data.theme.neutral1 }};
        border-radius: 40px;
        padding: 50px;
        padding-top:20px;
        border-style: solid;
        border-color: {{site.data.theme.primary}};
        margin-bottom:100px;
        max-width:575px;
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
    .discord {
        text-align: center;
        align-items: center;
        font-family: fira sans;
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
            flex-direction: column;
            justify-content: center;
            align-items: center;
            width: 100%;
        }
        .aside {
            padding-top: 40px;
            width: 100%;
            max-width: 575px;
        }

    }

</style>
<div class="about-content">
    <div class="main">
        {% include uofsc/team-intro.html %}
        {% include uofsc/game-intro.html %}
        {% include uofsc/discord.html %}
        {% include uofsc/officers.html %}
        {% include uofsc/sponsors.html %}
    </div>
    <div class="buffer"> </div>
    <div class="aside"> 
        <div class="sticky">
            <h1>Consider Getting Involved</h1>
            <p>
                You can directly contribute to our VEX U team's success by making a financial donation. Your support fuels our journey to victory in the world of competitive robotics. Click the link below to donate and help us reach new heights!
            </p>
            <a href="https://donate.sc.edu/AG/sfp/cec/vex-robotics-club">
                University of South Carolina Gamecock Robotics Giving Page
            </a>
            <h1>Volunteer/​Sponsorship Opportunities</h1>
            <p>
                We are still looking for sponsors and volunteers for our High School and Middle School Tournaments on December 2nd. If you are intereseted you can reach out to <a href="mailto:sovexu@mailbox.sc.edu">sovexu@mailbox.sc.edu</a>.
            </p>
        </div>
    </div>
</div>
