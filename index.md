<!DOCTYPE html>
<html>

<head>
    <title>Minimal Resume Template</title>
    <link rel="stylesheet" type="text/css" href="/styles.css">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <style>
        /*Load google font*/
        @import url("https://fonts.googleapis.com/css?family=Lato:300,400,700");

        /* Reset Styles */

        html,
        body,
        div,
        span,
        applet,
        object,
        iframe,
        h1,
        h2,
        h3,
        h4,
        h5,
        h6,
        p,
        blockquote,
        pre,
        a,
        abbr,
        acronym,
        address,
        big,
        cite,
        code,
        del,
        dfn,
        em,
        img,
        ins,
        kbd,
        q,
        s,
        samp,
        small,
        strike,
        strong,
        sub,
        sup,
        tt,
        var,
        b,
        u,
        i,
        center,
        dl,
        dt,
        dd,
        ol,
        ul,
        li,
        fieldset,
        form,
        label,
        legend,
        table,
        caption,
        tbody,
        tfoot,
        thead,
        tr,
        th,
        td,
        article,
        aside,
        canvas,
        details,
        embed,
        figure,
        figcaption,
        footer,
        header,
        hgroup,
        menu,
        nav,
        output,
        ruby,
        section,
        summary,
        time,
        mark,
        audio,
        video {
            margin: 0;
            padding: 0;
            border: 0;
            font-size: 100%;
            font: inherit;
            vertical-align: baseline;
        }

        /* HTML5 display-role reset for older browsers */
        article,
        aside,
        details,
        figcaption,
        figure,
        footer,
        header,
        hgroup,
        menu,
        nav,
        section {
            display: block;
        }

        a {
            text-decoration: none;
            text-transform: none;
            color: #4a90e2;
        }

        body {
            line-height: 1;
            font-family: lato, ubuntu, -apple-system, BlinkMacSystemFont, Segoe UI,
                Roboto, Oxygen, Ubuntu, Cantarell, Open Sans, Helvetica Neue, sans-serif;
            text-rendering: optimizeLegibility;
            -webkit-font-smoothing: antialiased;
            font-size: 19px;
            background-color: #fefefe;
            color: #04143a;
        }

        ol,
        ul {
            list-style: none;
        }

        blockquote,
        q {
            quotes: none;
        }

        blockquote:before,
        blockquote:after,
        q:before,
        q:after {
            content: "";
            content: none;
        }

        table {
            border-collapse: collapse;
            border-spacing: 0;
        }

        p {
            color: #15171a;
            font-size: 17;
            line-height: 31px;
        }

        strong {
            font-weight: 600;
        }

        div,
        footer {
            box-sizing: border-box;
        }

        /* Reset ends */

        /*Hero section*/

        .container {
            max-width: 1100px;
            height: auto;
            margin: 60px auto;
        }

        .hero {
            margin: 50px auto;
            position: relative;
        }

        h1.name {
            font-size: 70px;
            font-weight: 300;
            display: inline-block;
        }

        .job-title {
            vertical-align: top;
            background-color: #d9e7f8;
            color: #4a90e2;
            font-weight: 600;
            margin-top: 5px;
            margin-left: 20px;
            border-radius: 5px;
            display: inline-block;
            padding: 15px 25px;
        }

        .email {
            display: block;
            font-size: 24px;
            font-weight: 300;
            color: #81899c;
            margin-top: 10px;
        }

        .lead {
            font-size: 44px;
            font-weight: 300;
            margin-top: 60px;
            line-height: 55px;
        }

        /*hero ends*/

        /*skills & intrests*/

        .sections {
            vertical-align: top;
            display: inline-block;
            width: 49.7%;
            height: 50px;
        }

        .section-title {
            font-size: 20px;
            font-weight: 600;
            margin-bottom: 15px;
        }

        .list-card {
            margin: 30px 0;
        }

        .list-card .exp,
        .list-card div {
            display: inline-block;
            vertical-align: top;
        }

        .list-card .exp {
            margin-right: 15px;
            color: #4a90e2;
            font-weight: 600;
            width: 100px;
        }

        .list-card div {
            width: 70%;
        }

        .list-card h3 {
            font-size: 20px;
            font-weight: 600;
            color: #5b6a9a;
            line-height: 26px;
            margin-bottom: 8px;
        }

        .list-card div span {
            font-size: 16px;
            color: #81899c;
            line-height: 22px;
        }

        /*skill and intrests ends*/

        /* Achievements */

        .cards {
            max-width: 1120px;
            display: block;
            margin-top: 280px;
        }

        .card {
            width: 47.9%;
            height: 200px;
            background-color: #eef0f7;
            display: inline-block;
            margin: 7px 5px;
            vertical-align: top;
            border-radius: 10px;
            text-align: center;
            padding-top: 50px;
        }

        .card-active,
        .card:hover {
            transform: scale(1.02);
            transition: 0.5s;
            background-color: #fff;
            box-shadow: 0px 5px 50px -8px #ddd;
            cursor: pointer;
        }

        .skill-level {
            display: inline-block;
            max-width: 160px;
        }

        .skill-level span {
            font-size: 35px;
            font-weight: 300;
            color: #5b6a9a;
            vertical-align: top;
        }

        .skill-level h2 {
            font-size: 95px;
            font-weight: 300;
            display: inline-block;
            vertical-align: top;
            color: #5b6a9a;
            letter-spacing: -5px;
        }

        .skill-meta {
            vertical-align: top;
            display: inline-block;
            max-width: 300px;
            text-align: left;
            margin-top: 15px;
            margin-left: 15px;
        }

        .skill-meta h3 {
            font-size: 20px;
            font-weight: 800;
            color: #5b6a9a;
            margin-bottom: 5px;
        }

        .skill-meta span {
            color: #81899c;
            line-height: 20px;
            font-size: 16px;
        }

        #main_content_wrap {
            background-color: white;
        }

        /* Achievements ends */

        /* Timeline styles*/

        ol {
            position: relative;
            display: block;
            margin: 100px 0;
            height: 2px;
            background: #eef0f7;
        }

        ol::before,
        ol::after {
            content: "";
            position: absolute;
            top: -10px;
            display: block;
            width: 0;
            height: 0;
            border-radius: 10px;
            border: 0px solid #31708f;
        }

        ol::before {
            left: -5px;
        }

        ol::after {
            right: -10px;
            border: 0px solid transparent;
            border-right: 0;
            border-left: 20px solid #31708f;
            border-radius: 3px;
        }

        /* ---- Timeline elements ---- */
        li {
            position: relative;
            display: inline-block;
            float: left;
            width: 20%;
            height: 50px;
        }

        li .line {
            position: absolute;
            top: -47px;
            left: 1%;
            font-size: 20px;
            font-weight: 600;
            color: #04143a;
        }

        li .point {
            content: "";
            top: -7px;
            left: 0%;
            display: block;
            width: 8px;
            height: 8px;
            border: 4px solid #fff;
            border-radius: 10px;
            background: #4a90e2;
            position: absolute;
        }

        li .description {
            display: none;
            padding: 10px 0;
            margin-top: 20px;
            position: relative;
            font-weight: normal;
            z-index: 1;
            max-width: 95%;
            font-size: 18px;
            font-weight: 600;
            line-height: 25px;
            color: #5b6a9a;
        }

        .description::before {
            content: "";
            width: 0;
            height: 0;
            border-left: 5px solid transparent;
            border-right: 5px solid transparent;
            border-bottom: 5px solid #f4f4f4;
            position: absolute;
            top: -5px;
            left: 43%;
        }

        .timeline .date {
            font-size: 14px;
            color: #81899c;
            font-weight: 300;
        }

        /* ---- Hover effects ---- */
        li:hover {
            color: #48a4d2;
        }

        li .description {
            display: block;
        }

        div .inner {
            width: 100%;
        }

        #header_wrap {
            display: none;
        }

        .inner {
            max-width: none;
        }

        h2 {
            background: none;
        }

        /*timeline ends*/

        /* Media queries*/

        @media (max-width: 1024px) {
            .container {
                padding: 15px;
                margin: 0px auto;
            }

            .cards {
                margin-top: 250px;
            }
        }

        @media (max-width: 768px) {
            .container {
                padding: 15px;
                margin: 0px auto;
            }

            .cards {
                margin-top: 320px;
            }

            .card {
                padding: 15px;
                text-align: left;
            }

            .card h2 {
                font-size: 70px;
            }

            .card,
            .sections {
                width: 100%;
                height: auto;
                margin: 10px 0;
                float: left;
            }

            .timeline {
                border: none;
                background-color: rgba(0, 0, 0, 0);
            }

            .timeline li {
                margin-top: 70px;
                height: 150px;
            }
        }

        @media (max-width: 425px) {
            h1.name {
                font-size: 40px;
            }

            .card,
            .sections {
                width: 100%;
                height: auto;
                margin: 10px 0;
                float: left;
            }

            .timeline {
                display: none;
            }

            .job-title {
                position: absolute;
                font-size: 15px;
                top: -40px;
                right: 20px;
                padding: 10px;
            }

            .lead {
                margin-top: 15px;
                font-size: 20px;
                line-height: 28px;
            }

            .container {
                margin: 0px;
                padding: 0 15px;
            }

            footer {
                margin-top: 2050px;
            }
        }
    </style>

</head>

<body>

    <div class="container">
        <div class="hero">
            <h1 class="name"><strong>Sourav</strong> Kayal</h1>
            <span class="job-title">Lead Software Engineer</span>
            <span class="email">sourav.kayal@yahoo.com | <a
                    href="https://www.linkedin.com/in/sourav-kayal-80597338/">@LinkedIn</a></span>

            <h2 class="lead">Lead software engineer with 12+ experience in C# .NET Core, Python, LLM, GenAI and
                <a href="https://github.com/souravkayal?tab=repositories">more</a>
                !
            </h2>
        </div>
    </div>

    <!-- Timeeline -->
    <div class="container">
        <ol class="timeline">
            <li>
                <p class="line">Experiences</p>
                <span class="point"></span>
                <p class="description">
                    <a href="https://www.honeywell.com/us/en" target="_blank">Honeywell</a>
                </p>
                <span class="date">May, 2021 - Today</span>
            </li>

            <li>
                <span class="point"></span>
                <p class="description">
                    <a href="https://www.us.jll.com/" target="_blank">JLL</a>
                </p>
                <span class="date"> December, 2020 - May, 2021</span>
            </li>

            <li>
                <span class="point"></span>
                <p class="description">
                    <a href="https://www.walmart.com/" target="_blank">Walmart</a>
                </p>
                <span class="date"> Aug, 2017 - December, 2020</span>
            </li>

            <li>
                <span class="point"></span>
                <p class="description">
                    <a href="https://www.dell.com/en-in" target="_blank">DELL-EMC</a>
                </p>
                <span class="date">Aug, 2017 - December, 2020</span>
            </li>
            <li>
                <span class="point"></span>
                <p class="description">
                    <a href="https://www.timken.com/en-in/" target="_blank">Timken</a>
                </p>
                <span class="date">Mar, 2014 - Aug, 2015</span>
            </li>
        </ol>

    </div>
    <br />

    <!-- Skills and intrest section -->
    <div class="container">

        <div class="sections">
            <h2 class="section-title">Skills</h2>

            <div class="list-card">
                <span class="exp">+ 12 years</span>
                <div>
                    <h3>Programming & Tech</h3>
                    <span>C#, .NET Core, Python, Azure, Multi model DB, PostgreSQL, GenAI / Agentic AI and more </span>
                </div>
            </div>

            <div class="list-card">
                <span class="exp">+ 3 years</span>
                <div>
                    <h3>Design & Architecture</h3>
                    <span>Worked as design lead in various modules in multiple products.
                </div>
            </div>

            <div class="list-card">
                <span class="exp">+ 2 years</span>
                <div>
                    <h3>Leading a team</h3>
                    <span>Leading a core team of few developers. </span>
                </div>
            </div>

        </div>

        <div class="sections">
            <h2 class="section-title">Writings and Publications</h2>

            <div class="list-card">
                <div>
                    <h3><a href="https://medium.com/@ctrlcvprogrammer" target="_blank"> @medium </a></h3>
                    <h3><a href="https://www.csharp.com/members/sourav-kayal/articles-3" target="_blank">
                            @c-sharpcorner.com</a></h3>
                    <span></span>
                </div>
            </div>

            <div class="list-card">
                <div>
                    <h3>Patient (in-progress)</h3>
                    <span>Building Industrial Knowledge Graph</span> <br /><br />
                    <span>Mapping multiple asset moldel in uniformed visualization</span>
                </div>
            </div>
        </div>
    </div>

    <!-- Achievements -->
    <br />
    <div class="container cards">

        <div class="card">
            <div class="skill-level">
                <span>+</span>
                <h2>5</h2>
            </div>

            <div class="skill-meta">
                <h3>Fortune companys</h3>
                <span>I have worked for 5+ fortune companys and build applications which scale to millions of
                    customers</span>
            </div>
        </div>

        <div class="card">
            <div class="skill-level">
                <span>+</span>
                <h2>11</h2>
            </div>

            <div class="skill-meta">
                <h3>projects</h3>
                <span>Worked in 11+ projects using old to cutting edge stack across various sectiors including
                    oil & gas, retail, manufacturing</span>
            </div>
        </div>
    </div>


    <div class="container" width="100%">
        <div class="sections">
            <h2 class="section-title">Few certifications, I have completed recently.</h2>

            <div class="list-card">

                <div style="width: 100%;margin-bottom: 15px;">
                    <h5><a href="https://credentials.databricks.com/5b9cf798-baef-4ab3-854f-a8491836c67a#acc.FqYMnIyL"
                            target="_blank">
                            Academy Accreditation - Generative AI Fundamentals
                        </a>
                    </h5>
                </div>

                <div style="width: 100%;margin-bottom: 15px;">
                    <h2><a href="https://www.credly.com/badges/b7422961-71a1-4d06-bad9-13a240ff4035/linked_in_profile"
                            target="_blank">
                            Building AI-Powered Search with MongoDB Vector Search
                        </a>
                    </h2>
                </div>

                <div style="width: 100%;margin-bottom: 15px;">
                    <h2><a href="https://www.credly.com/badges/c4ebd0a7-0d22-4f38-8388-f8b5325448a4/linked_in_profile"
                            target="_blank">
                            Building RAG Apps Using MongoDB
                        </a>
                    </h2>
                </div>

                <div style="width: 100%;margin-bottom: 15px;">
                    <h2><a href="https://graphacademy.neo4j.com/c/10d0b8c2-4560-4c11-b087-703744478f70/"
                            target="_blank">
                            Neo4j Certified Professional
                        </a>
                    </h2>
                </div>

            </div>
        </div>
    </div>

    <br /><br /><br />
    <div class="container">
        <div class="sections">
            <h2 class="section-title">Books That Shaped My Thinking</h2>
            <div class="list-card">
                <div>
                    <h3>Programming and Leadership</h3>
                    <span>C# in depth - John Kits</span><br />
                    <span>Database Internals - Alex Petrov</span><br />
                    <span>System design - Alex Xu </span><br />
                    <span>The pragmetic programmer - Haunt Thomas </span><br />
                </div>
            </div>

            <div class="list-card">
                <div>
                    <h3>Self learning and growth mindset</h3>
                    <span>Atomic Habit - James Clear</span><br />
                    <span>Re Work - Jason Fried & David Heinemeier Hansson</span><br />
                </div>
            </div>

        </div>
    </div>

    <br /><br /><br /><br /><br />

    <div class="container">
        <div class="sections">
            <br /><br /><br />
            <span style="font-size: 16px; margin-top: 20px;">Coded by <a href="https://newtodesign.com/">New to design
                </a>
                Draft by <a href="#">Surav Kayal</a></span>
        </div>
    </div>
</body>


</html>
