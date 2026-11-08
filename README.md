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
    --text:#1e293b;
    --muted:#64748b;
    --accent:#2563eb;
    --accent-hover:#1d4ed8;
    --border:#e2e8f0;
    --shadow:0 4px 12px rgba(0,0,0,.08);
    --radius:14px;
    --max-width:1200px;
}

@media (prefers-color-scheme: dark){
    :root{
        --bg:#0f172a;
        --surface:#1e293b;
        --text:#f8fafc;
        --muted:#cbd5e1;
        --accent:#60a5fa;
        --accent-hover:#93c5fd;
        --border:#334155;
        --shadow:0 6px 18px rgba(0,0,0,.25);
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
    font-family:Inter, Segoe UI, sans-serif;
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
    z-index:100;
    background:var(--bg);
    border-bottom:1px solid var(--border);
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
    font-weight:700;
    color:var(--accent);
    font-size:1.1rem;
}

.nav-links{
    display:flex;
    gap:1.5rem;
    flex-wrap:wrap;
}

.nav-links a{
    color:var(--text);
    text-decoration:none;
    font-weight:500;
}

.nav-links a:hover{
    color:var(--accent);
}

/* HERO */

.hero{
    padding:4rem 0 2rem;
}

.hero h1{
    font-size:clamp(2.2rem, 5vw, 3.8rem);
    margin-bottom:1rem;
}

.hero p{
    max-width:800px;
    color:var(--muted);
    font-size:1.1rem;
}

/* SECTIONS */

section{
    margin-top:4rem;
}

h2{
    margin-bottom:1rem;
    border-bottom:2px solid var(--border);
    padding-bottom:.5rem;
}

h3{
    color:var(--accent);
}

/* SKILLS */

.skills-grid{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
    gap:1rem;
}

.skill-card{
    background:var(--surface);
    border:1px solid var(--border);
    border-radius:var(--radius);
    padding:1.25rem;
    box-shadow:var(--shadow);
}

.skill-card h3{
    margin-top:0;
}

/* PROJECTS */

.projects-grid{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(350px,1fr));
    gap:1.5rem;
}

.project-card{
    background:var(--surface);
    border:1px solid var(--border);
    border-radius:var(--radius);
    padding:1.5rem;
    box-shadow:var(--shadow);
    transition:transform .2s ease;
}

.project-card:hover{
    transform:translateY(-3px);
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
    padding:.3rem .7rem;
    margin:.2rem;
    border-radius:999px;
    font-size:.85rem;
}

.project-link{
    display:inline-block;
    margin-top:1rem;
    text-decoration:none;
    font-weight:600;
    color:var(--accent);
}

/* LISTS */

ul{
    padding-left:1.5rem;
}

li{
    margin-bottom:.45rem;
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
    color:var(--muted);
}

/* MOBILE */

@media(max-width:768px){

    .container{
        padding:1rem;
    }

    .nav-content{
        padding:1rem;
        flex-direction:column;
        gap:1rem;
    }

    .nav-links{
        justify-content:center;
    }

    .projects-grid{
        grid-template-columns:1fr;
    }
}
</style>
</head>

<body>

<header class="navbar">
    <nav class="nav-content" aria-label="Main navigation">
        <div class="logo">Desire Roslin Dziele</div>

        <div class="nav-links">
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
        systems programming, algorithms, and full-stack development. My projects focus
        on understanding how software works internally by implementing core concepts
        from first principles, including custom data structures, algorithm design,
        object-oriented systems, and application architecture.
    </p>

    <p>
        I enjoy building projects that combine solid engineering practices with
        practical functionality, emphasizing maintainability, testing,
        performance analysis, and clean code.
    </p>
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
        <li>Full-Stack Development</li>
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
                <li>CLion</li>
                <li>Visual Studio</li>
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
                persistence, and automated testing.
            </p>

            <div class="tech-stack">
                <span>Angular</span>
                <span>Express</span>
                <span>SQLite</span>
                <span>TypeScript</span>
            </div>

            <a class="project-link" href="https://github.com/roslindesiredziele-hash/person-management-system">
                View Repository →
            </a>
        </article>

        <article class="project-card">
            <h3>Algorithms Sorting Benchmark</h3>
            <p>
                Benchmarking suite implementing Bubble, Insertion, Merge,
                Quick, Heap, and Shell Sort with automated data collection,
                visualization, and performance analysis.
            </p>

            <div class="tech-stack">
                <span>C++</span>
                <span>Python</span>
                <span>Algorithms</span>
            </div>

            <a class="project-link" href="https://github.com/roslindesiredziele-hash/Algorithms-Sorting-Benchmark">
                View Repository →
            </a>
        </article>

        <article class="project-card">
            <h3>Vec</h3>
            <p>
                Educational C++ dynamic array implementation featuring manual
                memory management, copy and move semantics, and capacity growth.
            </p>

            <div class="tech-stack">
                <span>C++</span>
                <span>Memory Management</span>
                <span>Data Structures</span>
            </div>

            <a class="project-link" href="https://github.com/roslindesiredziele-hash/Vec">
                View Repository →
            </a>
        </article>

        <article class="project-card">
            <h3>Language Evolution Simulator</h3>
            <p>
                Object-oriented programming project demonstrating inheritance,
                polymorphism, abstraction, and automated testing with Catch2.
            </p>

            <div class="tech-stack">
                <span>C++</span>
                <span>OOP</span>
                <span>Catch2</span>
            </div>

            <a class="project-link" href="https://github.com/roslindesiredziele-hash/Language">
                View Repository →
            </a>
        </article>

        <article class="project-card">
            <h3>CVRPTW</h3>
            <p>
                Implementation of the Capacitated Vehicle Routing Problem with
                Time Windows focusing on route optimization and constraints.
            </p>

            <a class="project-link" href="https://github.com/roslindesiredziele-hash/CVRPTW">
                View Repository →
            </a>
        </article>

        <article class="project-card">
            <h3>IPv4Address</h3>
            <p>
                C++ implementation for parsing, validating, and manipulating
                IPv4 addresses using clean object-oriented abstractions.
            </p>

            <a class="project-link" href="https://github.com/roslindesiredziele-hash/IPv4Address">
                View Repository →
            </a>
        </article>

    </div>
</section>

<section id="learning">
    <h2>What I'm Currently Learning</h2>

    <ul>
        <li>Advanced C++</li>
        <li>Move Semantics and Resource Management</li>
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
        <li>Gain software engineering internship experience</li>
        <li>Prepare for Erasmus+ studies in Nancy (2026/2027)</li>
    </ul>
</section>

<section id="contact">
    <h2>Contact</h2>

    <p>
        <strong>GitHub:</strong>
        <a href="https://github.com/roslindesiredziele-hash">
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
        © 2026 Desire Roslin Dziele · Computer Science Student · University of Łódź
    </p>
</footer>

</main>
</body>
</html>