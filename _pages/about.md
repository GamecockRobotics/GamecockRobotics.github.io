---
layout: home
title: "About"
---
<div id="about-page">
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
            width: 30%;
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
            width: 50%;
            margin: 20px;
        }
        .row .video {
            width: 50%;
            min-width: 240px;
            margin-top: 100px;
        }
        @media (max-width: 1000px) {
            .main {
                width: 100%;
                order: 2;
            }
            .about-content {
                flex-direction: column;
            }
            .sidebar {
                width: 100%;
            }
            .sticky {
                position: static;
            }
            .row {
                flex-direction: column;
            }
            .row .text {
                width: 90%;
                margin-left: 5%;
            }
            .row .video {
                width: 90%;
                margin-left: 5%;
                margin-top: 0px;
            }
        }
    </style>
    <div class="about-content">
        <div class="main">
            <div class="row">
                <div class="text">
                    <h1>VEX Robotics: Spin Up</h1>
                    <p>
                        Vex is a head to head competition where teams compete with two robots to score more points than the other team. Teams design, build, program and drive the robots. Each year a different challenge is presented.
                    </p>
                    <p>
                        Gamecock Robotics was founded in 2021 as the robotics team for the University of South Carolina. The team has 11 members and 1 faculty advisor.
                    </p>
                </div>
                <div class="video">
                    {% include structure/video.html src="wIZgvVDZc2Y" %}
                </div>
            </div>
            {% include structure/news.html %}
        </div>
        <div class="sidebar">
            <div class="sticky">
                {% include structure/aside.html %}
            </div>
        </div>
    </div>
</div>