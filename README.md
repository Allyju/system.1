# system.1
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>M_in_X.Tech | Book-Style Site</title>
    <style>
        :root {
            --page-color: #f8f1e5;
            --text-color: #3a3226;
            --accent: #8b5a2b;
        }
        
        body {
            background-color: #e0d5c0;
            font-family: 'Georgia', serif;
            color: var(--text-color);
            line-height: 1.6;
            padding: 2rem;
        }
        
        .book {
            display: flex;
            max-width: 1200px;
            margin: 0 auto;
            box-shadow: 0 0 30px rgba(0,0,0,0.3);
        }
        
        .page {
            width: 50%;
            padding: 3rem;
            background: var(--page-color);
            position: relative;
            min-height: 80vh;
            box-shadow: inset 0 0 10px rgba(0,0,0,0.1);
        }
        
        .left-page {
            border-right: 1px solid #d0c4b0;
        }
        
        .right-page {
            border-left: 1px solid #d0c4b0;
        }
        
        .page-number {
            position: absolute;
            bottom: 1rem;
            font-size: 0.9rem;
            color: var(--accent);
        }
        
        .left-page .page-number {
            right: 2rem;
        }
        
        .right-page .page-number {
            left: 2rem;
        }
        
        h1, h2 {
            color: var(--accent);
            border-bottom: 1px solid #d0c4b0;
            padding-bottom: 0.5rem;
        }
        
        @media (max-width: 768px) {
            .book {
                flex-direction: column;
            }
            .page {
                width: 100%;
                min-height: auto;
                padding: 2rem;
            }
            .left-page {
                border-right: none;
                border-bottom: 1px solid #d0c4b0;
            }
        }
    </style>
</head>
<body>
    <div class="book">
        <!-- Left Page (Even) -->
        <div class="page left-page">
            <h1>M_in_X.Tech</h1>
            <p>Welcome to our digital knowledge book. This layout mimics the experience of reading a physical book while being fully responsive.</p>
            
            <h2>Chapter 1: Web Development</h2>
            <p>Learn modern web technologies including HTML, CSS, and JavaScript. Build responsive websites that work on all devices.</p>
            
            <ul>
                <li>HTML5 Semantic Elements</li>
                <li>CSS Grid and Flexbox</li>
                <li>JavaScript Fundamentals</li>
            </ul>
            
            <div class="page-number">2</div>
        </div>
        
        <!-- Right Page (Odd) -->
        <div class="page right-page">
            <h2>Chapter 2: Software Design</h2>
            <p>Master the principles of clean code and software architecture. Design systems that are maintainable and scalable.</p>
            
            <blockquote style="border-left: 3px solid var(--accent); padding-left: 1rem; font-style: italic;">
                "Good software design is about making simple choices that remain flexible as requirements evolve."
            </blockquote>
            
            <h3>Key Concepts:</h3>
            <ol>
                <li>SOLID Principles</li>
                <li>Design Patterns</li>
                <li>Test-Driven Development</li>
            </ol>
            
            <div class="page-number">3</div>
        </div>
    </div>
</body>
</html>
