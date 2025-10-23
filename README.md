<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>First Love</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            background-color: #ffe6f2;
            color: #333;
            line-height: 1.6;
        }
        header {
            background-color: #ff99cc;
            text-align: center;
            padding: 2rem;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }
        h1 {
            margin: 0;
            color: white;
            font-size: 2.5rem;
        }
        main {
            max-width: 800px;
            margin: 2rem auto;
            padding: 1rem;
        }
        .intro {
            background-color: #fff;
            padding: 1.5rem;
            border-radius: 10px;
            margin-bottom: 2rem;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
        }
        .content {
            text-align: center;
        }
        .love-image {
            max-width: 100%;
            height: auto;
            border-radius: 10px;
            margin: 1rem 0;
            transition: transform 0.3s ease;
        }
        .love-image:hover {
            transform: scale(1.05);
        }
        .quotes {
            background-color: #ffccdd;
            padding: 1.5rem;
            border-radius: 10px;
            font-style: italic;
            text-align: center;
        }
        form {
            background-color: #fff;
            padding: 1.5rem;
            border-radius: 10px;
            margin-bottom: 2rem;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
        }
        textarea {
            width: 100%;
            padding: 0.5rem;
            border: 1px solid #ccc;
            border-radius: 5px;
        }
        button {
            background-color: #ff99cc;
            color: white;
            border: none;
            padding: 0.5rem 1rem;
            border-radius: 5px;
            cursor: pointer;
        }
        button:hover {
            background-color: #ff66b3;
        }
        .stories {
            background-color: #fff;
            padding: 1.5rem;
            border-radius: 10px;
            margin-bottom: 2rem;
        }
        footer {
            text-align: center;
            padding: 1rem;
            background-color: #ff99cc;
            color: white;
            margin-top: 2rem;
        }
        @media (max-width: 600px) {
            h1 {
                font-size: 2rem;
            }
            main {
                padding: 0.5rem;
            }
        }
    </style>
</head>
<body>
    <header>
        <h1>The Magic of First Love</h1>
    </header>
    <main>
        <section class="intro">
            <p>First love is a whirlwind of emotions, butterflies in your stomach, and unforgettable memories. It's the spark that ignites the heart and teaches us about vulnerability, joy, and sometimes heartache.</p>
        </section>
        <section class="content">
            <h2>Memories to Cherish</h2>
            <p>Think back to that first crush, the nervous smiles, and the endless conversations. First love shapes who we are and reminds us of the beauty in new beginnings.</p>
            <img src="https://via.placeholder.com/600x400?text=First+Love" alt="A romantic image representing first love" class="love-image">
        </section>
        <section class="quotes">
            <blockquote>"The best and most beautiful things in the world cannot be seen or even touched—they must be felt with the heart." – Helen Keller</blockquote>
        </section>
        <form action="/submit" method="post">
            <h2>Share Your First Love Story</h2>
            <textarea name="story" rows="4" placeholder="Tell us about your first love..."></textarea><br><br>
            <button type="submit">Submit Story</button>
        </form>
        <section class="stories">
            <h2>Shared Stories</h2>
            {% for story in stories %}
                <p>{{ story }}</p>
            {% endfor %}
        </section>
    </main>
    <footer>
        <p>&copy; 2023 First Love Website. Made with love and Python.</p>
    </footer>
</body>
</html>