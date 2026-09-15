# antdavis.github.io

```css
/* =========================================
   GENERAL
========================================= */

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html {
    scroll-behavior: smooth;
}

body {
    font-family: Arial, Helvetica, sans-serif;
    background: #0b0d12;
    color: #f5f5f5;
    line-height: 1.6;
    transition: background 0.3s, color 0.3s;
}

a {
    text-decoration: none;
    color: inherit;
}


/* =========================================
   NAVIGATION
========================================= */

.navbar {
    position: sticky;
    top: 0;
    z-index: 1000;

    display: flex;
    align-items: center;
    justify-content: space-between;

    padding: 18px 8%;

    background: rgba(11, 13, 18, 0.9);
    backdrop-filter: blur(12px);

    border-bottom: 1px solid #252934;
}

.logo {
    width: 45px;
    height: 45px;

    display: flex;
    align-items: center;
    justify-content: center;

    border-radius: 50%;

    background: #ffffff;
    color: #0b0d12;

    font-weight: bold;
}

.navbar nav {
    display: flex;
    gap: 30px;
}

.navbar nav a {
    color: #c4c7d0;
    font-size: 15px;

    transition: color 0.2s;
}

.navbar nav a:hover {
    color: #ffffff;
}

.theme-button {
    border: none;
    background: transparent;

    font-size: 20px;
    cursor: pointer;
}


/* =========================================
   HERO
========================================= */

.hero {
    min-height: 90vh;

    display: flex;
    align-items: center;
    justify-content: space-between;

    gap: 80px;

    padding: 80px 10%;
}

.hero-content {
    max-width: 700px;
}

.eyebrow {
    color: #8f96a3;

    font-size: 13px;
    font-weight: bold;

    letter-spacing: 3px;

    margin-bottom: 15px;
}

.hero h1 {
    font-size: clamp(48px, 7vw, 88px);
    line-height: 1.05;

    margin-bottom: 20px;
}

.hero h1 span {
    color: #8f96a3;
}

.hero h2 {
    font-size: 24px;
    color: #c4c7d0;

    margin-bottom: 20px;
}

.hero-description {
    max-width: 600px;

    color: #9298a5;
    font-size: 18px;

    margin-bottom: 35px;
}

.hero-buttons {
    display: flex;
    gap: 15px;
    flex-wrap: wrap;
}


/* =========================================
   BUTTONS
========================================= */

.button {
    display: inline-block;

    padding: 13px 22px;

    border-radius: 8px;

    font-weight: bold;

    transition:
        transform 0.2s,
        background 0.2s;
}

.button:hover {
    transform: translateY(-3px);
}

.primary {
    background: #ffffff;
    color: #0b0d12;
}

.secondary {
    border: 1px solid #343946;
    color: #ffffff;
}

.secondary:hover {
    background: #181b23;
}


/* =========================================
   PROFILE CARD
========================================= */

.hero-card {
    width: 300px;

    padding: 40px 30px;

    text-align: center;

    border: 1px solid #292d38;
    border-radius: 20px;

    background: #11141b;

    box-shadow: 0 20px 60px rgba(0,0,0,0.3);
}

.profile-circle {
    width: 140px;
    height: 140px;

    margin: auto;
    margin-bottom: 25px;

    display: flex;
    align-items: center;
    justify-content: center;

    border-radius: 50%;

    background: #ffffff;
    color: #0b0d12;

    font-size: 35px;
    font-weight: bold;
}

.hero-card h3 {
    font-size: 23px;
    margin-bottom: 5px;
}

.hero-card p {
    color: #858b98;
}


/* =========================================
   SECTIONS
========================================= */

.section {
    padding: 110px 10%;
}

.alternate {
    background: #10131a;
}

.section-heading {
    max-width: 700px;
    margin-bottom: 55px;
}

.section-heading h2 {
    font-size: 45px;
    line-height: 1.1;

    margin-bottom: 15px;
}

.section-heading > p:last-child {
    color: #8d93a0;
}


/* =========================================
   ABOUT
========================================= */

.about-grid {
    display: grid;

    grid-template-columns: 1.4fr 1fr;

    gap: 70px;
}

.about-text p {
    color: #aeb2bc;
    font-size: 18px;

    margin-bottom: 20px;
}

.about-info {
    display: flex;
    flex-direction: column;
    gap: 15px;
}

.info-card {
    display: flex;
    align-items: center;
    gap: 18px;

    padding: 20px;

    border: 1px solid #292d38;
    border-radius: 12px;

    background: #11141b;
}

.info-card > span {
    font-size: 27px;
}

.info-card h3 {
    font-size: 17px;
}

.info-card p {
    color: #858b98;
}


/* =========================================
   SKILLS
========================================= */

.skills-grid {
    display: grid;

    grid-template-columns: repeat(4, 1fr);

    gap: 20px;
}

.skill-card {
    padding: 30px;

    border: 1px solid #292d38;
    border-radius: 15px;

    background: #11141b;

    transition:
        transform 0.2s,
        border-color 0.2s;
}

.skill-card:hover {
    transform: translateY(-6px);
    border-color: #5b6170;
}

.skill-icon {
    font-size: 32px;
    margin-bottom: 20px;
}

.skill-card h3 {
    margin-bottom: 10px;
}

.skill-card p {
    color: #858b98;
}


/* =========================================
   PROJECTS
========================================= */

.projects-grid {
    display: grid;

    grid-template-columns: repeat(3, 1fr);

    gap: 25px;
}

.project-card {
    position: relative;

    padding: 35px;

    min-height: 300px;

    border: 1px solid #292d38;
    border-radius: 15px;

    background: #11141b;

    transition: transform 0.2s;
}

.project-card:hover {
    transform: translateY(-6px);
}

.project-number {
    color: #555b68;

    font-size: 14px;
    font-weight: bold;

    margin-bottom: 30px;
}

.project-card h3 {
    font-size: 25px;

    margin-bottom: 15px;
}

.project-card p {
    color: #858b98;

    margin-bottom: 25px;
}

.tags {
    display: flex;
    gap: 8px;
    flex-wrap: wrap;
}

.tags span {
    padding: 5px 10px;

    border-radius: 5px;

    background: #20242d;

    color: #aeb2bc;

    font-size: 12px;
}


/* =========================================
   GOALS
========================================= */

.goals {
    background: #10131a;
}

.goal-box {
    max-width: 850px;

    padding: 40px;

    border-left: 3px solid #ffffff;

    background: #11141b;
}

.goal-box p {
    color: #aeb2bc;

    font-size: 19px;

    margin-bottom: 20px;
}

.goal-box p:last-child {
    margin-bottom: 0;
}


/* =========================================
   CONTACT
========================================= */

.contact {
    text-align: center;
}

.contact .section-heading {
    margin-left: auto;
    margin-right: auto;
}

.contact-buttons {
    display: flex;
    justify-content: center;

    gap: 15px;

    flex-wrap: wrap;
}


/* =========================================
   FOOTER
========================================= */

footer {
    padding: 30px 10%;

    text-align: center;

    border-top: 1px solid #252934;

    color: #666c79;

    font-size: 14px;
}


/* =========================================
   LIGHT MODE
========================================= */

body.light {
    background: #f5f5f5;
    color: #111111;
}

body.light .navbar {
    background: rgba(245,245,245,0.9);
    border-color: #dddddd;
}

body.light .navbar nav a {
    color: #555555;
}

body.light .hero h1 span {
    color: #666666;
}

body.light .hero h2,
body.light .hero-description,
body.light .about-text p {
    color: #555555;
}

body.light .hero-card,
body.light .info-card,
body.light .skill-card,
body.light .project-card,
body.light .goal-box {
    background: #ffffff;
    border-color: #dddddd;
}

body.light .alternate,
body.light .goals {
    background: #eeeeee;
}

body.light .secondary {
    color: #111111;
    border-color: #cccccc;
}


/* =========================================
   MOBILE
========================================= */

@media (max-width: 900px) {

    .navbar {
        padding: 15px 5%;
    }

    .navbar nav {
        gap: 15px;
    }

    .hero {
        flex-direction: column;
        text-align: center;

        padding: 70px 6%;
    }

    .hero-description {
        margin-left: auto;
        margin-right: auto;
    }

    .hero-buttons {
        justify-content: center;
    }

    .about-grid {
        grid-template-columns: 1fr;
    }

    .skills-grid {
        grid-template-columns: repeat(2, 1fr);
    }

    .projects-grid {
        grid-template-columns: 1fr;
    }

}


@media (max-width: 600px) {

    .navbar nav {
        display: none;
    }

    .section {
        padding: 80px 6%;
    }

    .hero {
        min-height: auto;
    }

    .hero-card {
        width: 100%;
        max-width: 320px;
    }

    .skills-grid {
        grid-template-columns: 1fr;
    }

    .section-heading h2 {
        font-size: 36px;
    }

}
```

