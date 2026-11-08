<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Desire Roslin Dziele | Computer Science Student</title>

<style>
:root{
    --bg:#ffffff;
    --surface:#f8fafc;
    --surface-alt:#eef2ff;
    --text:#1e293b;
    --muted:#64748b;
    --accent:#2563eb;
    --accent-hover:#1d4ed8;
    --border:#e2e8f0;
    --shadow:0 4px 12px rgba(0,0,0,.08);
    --shadow-hover:0 10px 24px rgba(0,0,0,.12);
    --radius:14px;
    --max-width:1200px;
}

@media (prefers-color-scheme: dark){
    :root{
        --bg:#0f172a;
        --surface:#1e293b;
        --surface-alt:#172554;
        --text:#f8fafc;
        --muted:#cbd5e1;
        --accent:#60a5fa;
        --accent-hover:#93c5fd;
        --border:#334155;
        --shadow:0 6px 18px rgba(0,0,0,.25);
        --shadow-hover:0 12px 28px rgba(0,0,0,.35);
    }
}

*{
    box-sizing:border-box;
}

html{
    scroll-behavior:smooth;
}

body{
    margin:0;
    background:var(--bg);
    color:var(--text);
    font-family:Inter, Segoe UI, Roboto, Helvetica, Arial, sans-serif;
    line-height:1.7;
}

.container{
    max-width:var(--max-width);
    margin:auto;
    padding:2rem;
}

/* NAVIGATION */

.navbar{
    position:sticky;
    top:0;
    z-index:1000;
    background:rgba(255,255,255,.9);
    backdrop-filter:blur(12px);
    border-bottom:1px solid var(--border);
}

@media (prefers-color-scheme: dark){
    .navbar{
        background:rgba(15,23,42,.9);
    }
}

.nav-content{
    max-width:var(--max-width);
    margin:auto;
    padding:1rem 2rem;
    display:flex;
    justify-content:space-between;
    align-items:center;
}

.logo{
    font-size:1.1rem;
    font-weight:700;
    color:var(--accent);
    text-decoration:none;
}

.nav-links{
    display:flex;
    gap:1.5rem;
}

.nav-links a{
    color:var(--text);
    text-decoration:none;
    font-weight:500;
}

.nav-links a:hover{
    color:var(--accent);
}

.menu-toggle{
    display:none;
    border:none;
    background:none;
    color:var(--text);
    cursor:pointer;
    font-size:1.5rem;
    padding:.5rem;
    border-radius:8px;
}

.menu-toggle:hover{
    background:var(--surface);
}

.menu-toggle:focus-visible,
.nav-links a:focus-visible,
.project-link:focus-visible{
    outline:3px solid var(--accent);
    outline-offset:3px;
}

/* HERO */

.hero{
    padding:5rem 0 3rem;
}

.hero h1{
    font-size:clamp(2.5rem,5vw,4rem);
    line-height:1.15;
    margin-bottom:1rem;
}

.hero p{
    max-width:850px;
    color:var(--muted);
    font-size:1.1rem;
}

.badges{
    margin-top:1.5rem;
}

.badge{
    display:inline-block;
    background:var(--surface-alt);
    color:var(--accent);
    border:1px solid var(--border);
    padding:.45rem .85rem;
    border-radius:999px;
    margin:.25rem;
    font-size:.9rem;
    font-weight:600;
}

/* SECTIONS */

section{
    margin-top:4rem;
}

h2{
    margin-bottom:1.5rem;
    border-bottom:2px solid var(--border);
    padding-bottom:.6rem;
}

h3{
    color:var(--accent);
}

/* SKILLS */

.skills-grid{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
    gap:1.25rem;
}

.skill-card{
    background:var(--surface);
    border:1px solid var(--border);
    border-radius:var(--radius);
    padding:1.5rem;
    box-shadow:var(--shadow);
}

.skill-card h3{
    margin-top:0;
}

/* PROJECTS */

.projects-grid{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(340px,1fr));
    gap:1.5rem;
}

.project-card{
    background:var(--surface);
    border:1px solid var(--border);
    border-radius:var(--radius);
    padding:1.5rem;
    box-shadow:var(--shadow);
    transition:.25s;
}

.project-card:hover{
    transform:translateY(-4px);
    box-shadow:var(--shadow-hover);
}

.project-card h3{
    margin-top:0;
}

.tech-stack{
    margin-top:1rem;
}

.tech-stack span{
    display:inline-block;
    background:var(--accent);
    color:white;
    padding:.35rem .75rem;
    border-radius:999px;
    margin:.2rem;
    font-size:.85rem;
}

.project-link{
    display:inline-block;
    margin-top:1rem;
    color:var(--accent);
    font-weight:600;
    text-decoration:none;
}

.project-link:hover{
    text-decoration:underline;
}

/* LISTS */

ul{
    padding-left:1.25rem;
}

li{
    margin-bottom:.5rem;
}

/* LINKS */

a{
    color:var(--accent);
}

a:hover{
    color:var(--accent-hover);
}

/* FOOTER */

footer{
    margin-top:5rem;
    border-top:1px solid var(--border);
    padding-top:2rem;
    text-align:center;
    color:var(--muted);
}

/* MOBILE */

@media(max-width:768px){

    .container{
        padding:1rem;
    }

    .menu-toggle{
        display:block;
    }

    .nav-content{
        padding:1rem;
        flex-wrap:wrap;
    }

    .nav-links{
        display:none;
        width:100%;
        flex-direction:column;
        margin-top:1rem;
    }

    .nav-links.open{
        display:flex;
    }

    .nav-links a{
        padding:.85rem;
        background:var(--surface);
        border-radius:8px;
    }

    .projects-grid{
        grid-template-columns:1fr;
    }
}

@media(prefers-reduced-motion: reduce){
    *{
        scroll-behavior:auto;
        transition:none !important;
        animation:none !important;
    }
}
</style>
</head>

<body>

<header class="navbar">
    <nav class="nav-content" aria-label="Main navigation">

        <a href="#about" class="logo">
            Desire Roslin Dziele
        </a>

        <button
            class="menu-toggle"
            id="menuButton"
            aria-controls="mobile-menu"
            aria-expanded="false"
            aria-label="Toggle navigation menu">
            ☰
        </button>

        <div class="nav-links" id="mobile-menu">
            <a href="#about">About</a>
            <a href="#interests">Interests</a>
            <a href="#skills">Skills</a>
            <a href="#projects">Projects</a>
            <a href="#learning">Learning</a>
            <a href="#goals">Goals</a>
            <a href="#contact">Contact</a>
        </div>

    </nav>
</header>

<main class="container">

<section class="hero" id="about">
    <h1>Computer Science Student at the University of Łódź</h1>

    <p>
        I am a Computer Science student with a strong interest in software engineering,
        systems programming, algorithms, and full-stack development. My projects focus on
        understanding how software works internally through custom data structures,
        algorithm implementation, object-oriented systems, and application architecture.
    </p>

    <p>
        I enjoy building software that combines strong engineering principles with
        practical functionality, maintainability, testing, and performance analysis.
    </p>

    <div class="badges">
        <span class="badge">C++</span>
        <span class="badge">TypeScript</span>
        <span class="badge">Angular</span>
        <span class="badge">Express.js</span>
        <span class="badge">SQLite</span>
        <span class="badge">Python</span>
        <span class="badge">Algorithms</span>
        <span class="badge">Testing</span>
    </div>
</section>

<section id="interests">
    <h2>Areas of Interest</h2>

    <ul>
        <li>Software Engineering</li>
        <li>Modern C++</li>
        <li>Data Structures and Algorithms</li>
        <li>Systems Programming</li>
        <li>Object-Oriented Design</li>
        <li>Software Architecture</li>
        <li>Full-Stack Web Development</li>
        <li>Database Systems</li>
        <li>Automated Testing</li>
        <li>Performance Analysis</li>
    </ul>
</section>

<section id="skills">
    <h2>Technical Skills</h2>

    <div class="skills-grid">

        <article class="skill-card">
            <h3>Programming Languages</h3>
            <ul>
                <li>C++</li>
                <li>TypeScript</li>
                <li>Python</li>
                <li>JavaScript</li>
                <li>SQL</li>
            </ul>
        </article>

        <article class="skill-card">
            <h3>Web Development</h3>
            <ul>
                <li>Angular</li>
                <li>Express.js</li>
                <li>REST APIs</li>
                <li>HTML</li>
                <li>CSS</li>
            </ul>
        </article>

        <article class="skill-card">
            <h3>Testing</h3>
            <ul>
                <li>Catch2</li>
                <li>Vitest</li>
                <li>Supertest</li>
            </ul>
        </article>

        <article class="skill-card">
            <h3>Tools</h3>
            <ul>
                <li>Git</li>
                <li>GitHub</li>
                <li>VS Code</li>
                <li>Visual Studio</li>
                <li>CLion</li>
                <li>Postman</li>
            </ul>
        </article>

    </div>
</section>

<section id="projects">
    <h2>Selected Projects</h2>

    <div class="projects-grid">

        <article class="project-card">
            <h3>Person Management System</h3>
            <p>
                Full-stack CRUD application built with Angular, Express.js,
                SQLite, and TypeScript featuring REST APIs, validation,
                persistence, automated testing, and sample-data generation.
            </p>

            <div class="tech-stack">
                <span>Angular</span>
                <span>Express</span>
                <span>SQLite</span>
                <span>TypeScript</span>
            </div>

            <a class="project-link" target="_blank"
               href="https://github.com/roslindesiredziele-hash/person-management-system">
               View Repository →
            </a>
        </article>

        <article class="project-card">
            <h3>Algorithms Sorting Benchmark</h3>
            <p>
                Performance-analysis project implementing Bubble, Insertion,
                Merge, Quick, Heap, and Shell Sort with automated benchmarking,
                CSV export, visualization, and complexity analysis.
            </p>

            <div class="tech-stack">
                <span>C++</span>
                <span>Python</span>
                <span>Algorithms</span>
            </div>

            <a class="project-link" target="_blank"
               href="https://github.com/roslindesiredziele-hash/Algorithms-Sorting-Benchmark">
               View Repository →
            </a>
        </article>

        <article class="project-card">
            <h3>Vec</h3>
            <p>
                Educational implementation of a dynamic array featuring manual
                memory management, capacity growth, copy/move semantics,
                bounds checking, and custom container behavior.
            </p>

            <div class="tech-stack">
                <span>C++</span>
                <span>Data Structures</span>
                <span>Memory Management</span>
            </div>

            <a class="project-link" target="_blank"
               href="https://github.com/roslindesiredziele-hash/Vec">
               View Repository →
            </a>
        </article>

        <article class="project-card">
            <h3>Language Evolution Simulator</h3>
            <p>
                Object-oriented programming project demonstrating abstraction,
                inheritance, polymorphism, virtual functions, and automated
                testing with Catch2.
            </p>

            <div class="tech-stack">
                <span>C++</span>
                <span>OOP</span>
                <span>Catch2</span>
            </div>

            <a class="project-link" target="_blank"
               href="https://github.com/roslindesiredziele-hash/Language">
               View Repository →
            </a>
        </article>

        <article class="project-card">
            <h3>CVRPTW</h3>
            <p>
                Implementation of the Capacitated Vehicle Routing Problem with
                Time Windows focusing on route optimization and constraint
                handling.
            </p>

            <a class="project-link" target="_blank"
               href="https://github.com/roslindesiredziele-hash/CVRPTW">
               View Repository →
            </a>
        </article>

        <article class="project-card">
            <h3>IPv4Address & CitiesDistance</h3>
            <p>
                Utility-focused C++ projects covering IPv4 validation,
                parsing, manipulation, and geographic distance calculations
                using reusable object-oriented abstractions.
            </p>

            <a class="project-link" target="_blank"
               href="https://github.com/roslindesiredziele-hash">
               View Repositories →
            </a>
        </article>

    </div>
</section>

<section id="learning">
    <h2>What I'm Currently Learning</h2>

    <ul>
        <li>Advanced C++</li>
        <li>Move Semantics and Resource Management</li>
        <li>Algorithms and Computational Complexity</li>
        <li>Software Architecture</li>
        <li>Design Patterns</li>
        <li>Database Design</li>
        <li>Angular Ecosystem</li>
        <li>Backend Development with Express.js</li>
    </ul>
</section>

<section id="goals">
    <h2>Current Goals</h2>

    <ul>
        <li>Build production-quality software projects</li>
        <li>Strengthen software engineering fundamentals</li>
        <li>Deepen knowledge of algorithms and data structures</li>
        <li>Expand full-stack development experience</li>
        <li>Obtain a software engineering internship</li>
        <li>Prepare for Erasmus+ studies in Nancy (2026/2027)</li>
        <li>Develop a portfolio showcasing both systems and application development</li>
    </ul>
</section>

<section id="contact">
    <h2>Contact</h2>

    <p>
        <strong>GitHub:</strong>
        <a href="https://github.com/roslindesiredziele-hash" target="_blank">
            github.com/roslindesiredziele-hash
        </a>
    </p>

    <p>
        <strong>Email:</strong>
        <a href="mailto:roslindesiredziele@gmail.com">
            roslindesiredziele@gmail.com
        </a>
    </p>
</section>

<footer>
    <p>
        © 2026 Desire Roslin Dziele · University of Łódź · Computer Science
    </p>
</footer>

</main>

<script>
const menuButton = document.getElementById("menuButton");
const mobileMenu = document.getElementById("mobile-menu");

menuButton.addEventListener("click", () => {
    const expanded =
        menuButton.getAttribute("aria-expanded") === "true";

    menuButton.setAttribute(
        "aria-expanded",
        String(!expanded)
    );

    mobileMenu.classList.toggle("open");
});

document.addEventListener("keydown", (event) => {
    if (
        event.key === "Escape" &&
        mobileMenu.classList.contains("open")
    ) {
        mobileMenu.classList.remove("open");
        menuButton.setAttribute("aria-expanded", "false");
        menuButton.focus();
    }
});

mobileMenu.querySelectorAll("a").forEach(link => {
    link.addEventListener("click", () => {
        if (window.innerWidth <= 768) {
            mobileMenu.classList.remove("open");
            menuButton.setAttribute("aria-expanded", "false");
        }
    });
});
</script>

</body>
</html>