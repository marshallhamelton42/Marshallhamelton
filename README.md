<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Marshall Hamelton - Ministry of Truth</title>
    <style>
        :root {
            --primary: #2c3e50;
            --secondary: #1a5276;
            --accent: #3498db;
            --light: #f8f9fa;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Merriweather', serif;
        }

        body {
            line-height: 1.8;
            color: #333;
            background: var(--light);
        }

        header {
            background: var(--primary);
            color: white;
            padding: 2rem;
            text-align: center;
            border-bottom: 5px solid var(--secondary);
        }

        nav {
            display: flex;
            justify-content: center;
            gap: 2rem;
            padding: 1rem;
            background: var(--secondary);
            flex-wrap: wrap;
        }

        nav a {
            color: white;
            text-decoration: none;
            padding: 1rem;
            transition: all 0.3s ease;
        }

        nav a:hover {
            background: var(--accent);
        }

        .hero {
            text-align: center;
            padding: 6rem 2rem;
            background: linear-gradient(rgba(44, 62, 80, 0.9), rgba(44, 62, 80, 0.9)), url('https://images.unsplash.com/photo-1450101499163-c8848c66ca85');
            background-size: cover;
            color: white;
        }

        .section {
            padding: 4rem 2rem;
            max-width: 1200px;
            margin: 0 auto;
        }

        .scripture-card {
            background: white;
            padding: 2rem;
            border-radius: 10px;
            margin: 2rem 0;
            box-shadow: 0 3px 15px rgba(0,0,0,0.1);
            border-left: 5px solid var(--accent);
        }

        .ministry-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            margin-top: 2rem;
        }

        .blog-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
            gap: 2rem;
            margin-top: 2rem;
        }

        .blog-post {
            background: white;
            padding: 1.5rem;
            border-radius: 8px;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
        }

        footer {
            background: var(--primary);
            color: white;
            text-align: center;
            padding: 3rem 2rem;
            margin-top: 4rem;
        }

        .contact-form {
            max-width: 600px;
            margin: 2rem auto;
            background: white;
            padding: 2rem;
            border-radius: 10px;
        }

        input, textarea, button {
            width: 100%;
            padding: 1rem;
            margin: 1rem 0;
            border: 2px solid #ddd;
            border-radius: 5px;
            font-size: 1rem;
        }

        button {
            background: var(--accent);
            color: white;
            font-weight: bold;
            cursor: pointer;
            transition: all 0.3s ease;
        }

        button:hover {
            background: #2471a3;
        }

        @media (max-width: 768px) {
            .section {
                padding: 2rem 1rem;
            }
            nav {
                gap: 0.5rem;
            }
        }
    </style>
    <link href="https://fonts.googleapis.com/css2?family=Merriweather:wght@400;700&display=swap" rel="stylesheet">
</head>
<body>
    <header>
        <h1>Marshall Hamelton</h1>
        <p>"I am the way, the truth, and the life" - John 14:6</p>
    </header>

    <nav>
        <a href="#home">Home</a>
        <a href="#beliefs">Core Beliefs</a>
        <a href="#ministry">Ministry</a>
        <a href="#blog">Teachings</a>
        <a href="#contact">Contact</a>
    </nav>

    <main>
        <section class="hero" id="home">
            <h2>Proclaiming Christ's Redemptive Work</h2>
            <p>"For the Son of man came to seek and to save the lost" - Luke 19:10</p>
        </section>

        <section class="section" id="beliefs">
            <div class="scripture-card">
                <h2>Statement of Faith</h2>
                <p>"All Scripture is breathed out by God..." - 2 Timothy 3:16 (ESV)</p>
                <ul>
                    <li>Born-again believer in Christ Jesus (John 3:3)</li>
                    <li>Believes in the Triune God: Father, Son, and Holy Spirit</li>
                    <li>Adheres to apostolic doctrine (Acts 2:42)</li>
                    <li>Affirms the divine inspiration of Scripture</li>
                    <li>Confesses Jesus as the only way to salvation (John 14:6)</li>
                </ul>
            </div>

            <div class="scripture-card">
                <h3>The Incarnate Word</h3>
                <p>"And the Word became flesh and dwelt among us..." - John 1:14</p>
                <p>We affirm Christ's divine nature and incarnation as the only begotten Son of the Father, full of grace and truth.</p>
            </div>
        </section>

        <section class="section" id="ministry">
            <h2>Ministry Focus</h2>
            <div class="ministry-grid">
                <div class="scripture-card">
                    <h3>Evangelism</h3>
                    <p>"For God so loved the world..." - John 3:16</p>
                    <ul>
                        <li>Proclaiming the Gospel to unbelievers</li>
                        <li>Community outreach programs</li>
                        <li>Apologetics and defense of the faith</li>
                    </ul>
                </div>
                
                <div class="scripture-card">
                    <h3>Discipleship</h3>
                    <p>"As newborn infants, long for the pure spiritual milk..." - 1 Peter 2:2</p>
                    <ul>
                        <li>Expository Bible teaching</li>
                        <li>Spiritual growth resources</li>
                        <li>Leadership training programs</li>
                    </ul>
                </div>
            </div>
        </section>

        <section class="section" id="blog">
            <h2>Recent Teachings</h2>
            <div class="blog-container" id="blog-posts">
                <!-- Dynamic content will load here -->
                <div class="loading">Loading teachings...</div>
            </div>
        </section>

        <section class="section" id="contact">
            <div class="contact-form">
                <h2>Connect With Marshall</h2>
                <form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
                    <input type="text" name="name" placeholder="Your Name" required>
                    <input type="email" name="email" placeholder="Your Email" required>
                    <textarea name="message" placeholder="Your Message" rows="6" required></textarea>
                    <button type="submit">Send Message</button>
                </form>
            </div>
        </section>
    </main>

    <footer>
        <div style="max-width: 800px; margin: 0 auto;">
            <p>Follow the Ministry:</p>
            <div style="margin: 1rem 0;">
                <a href="https://activepurposewriter.blogspot.com" target="_blank" style="color: white; margin: 0 1rem;">Blog</a>
                <a href="https://christianleaders.org/my/" target="_blank" style="color: white; margin: 0 1rem;">CLI Profile</a>
            </div>
            <p style="margin-top: 2rem;">&copy; 2024 Marshall Hamelton. Soli Deo Gloria.</p>
        </div>
    </footer>

    <script>
        // Blog Integration
        const RSS_FEED = 'YOUR_RSS_FEED_URL';

        async function loadBlogPosts() {
            try {
                const response = await fetch(RSS_FEED);
                const data = await response.json();
                
                const container = document.getElementById('blog-posts');
                container.innerHTML = '';
                
                data.items.forEach(post => {
                    const postEl = document.createElement('div');
                    postEl.className = 'blog-post';
                    postEl.innerHTML = `
                        <h3>${post.title}</h3>
                        <div style="color: #666; margin: 0.5rem 0;">
                            ${new Date(post.pubDate).toLocaleDateString()}
                        </div>
                        <div style="margin: 1rem 0;">
                            ${post.description}
                        </div>
                        <a href="${post.link}" target="_blank" style="color: var(--accent);">Continue Reading →</a>
                    `;
                    container.appendChild(postEl);
                });
            } catch (error) {
                console.error('Error loading content:', error);
                document.getElementById('blog-posts').innerHTML = `
                    <div class="scripture-card">
                        <p>Visit the <a href="https://activepurposewriter.blogspot.com" target="_blank">full blog</a> for all teachings.</p>
                    </div>
                `;
            }
        }

        // Initialize
        window.addEventListener('DOMContentLoaded', () => {
            loadBlogPosts();
        });
    </script>
</body>
</html>
