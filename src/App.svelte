<script>
  import { onMount } from 'svelte';
  let name = "Nithya 💻💗";
  let text = "";
  let index = 0;

  const typeWriter = () => {
    if (index < name.length) {
      text += name.charAt(index);
      index++;
      setTimeout(typeWriter, 100);
    }
  };

  onMount(() => {
    typeWriter();
  });
</script>

<style>
  :global(body) {
    font-family: 'Comic Sans MS', cursive, sans-serif;
    background: url('https://i.pinimg.com/750x/0d/81/07/0d8107683560f14b87d3241c45c04dfc.jpg');
    background-size: cover;
    margin: 0;
    padding: 0;
  }

  .container {
    max-width: 600px;
    margin: auto;
    background: rgba(255, 255, 255, 0.8);
    padding: 2rem;
    border-radius: 20px;
    margin-top: 4rem;
    box-shadow: 0 10px 25px rgba(0, 0, 0, 0.1);
  }

  header {
    text-align: center;
    margin-bottom: 2rem;
  }

  h1 {
    font-size: 2rem;
    color: #ff66cc;
    margin-bottom: 1rem;
  }

  img {
    width: 150px;
    border-radius: 50%;
    border: 4px  #ffb6c1;
  }

  h2 {
    color: #ff66cc;
    margin-top: 2rem;
  }

  p, li, a {
    font-size: 1rem;
    color: #444;
    line-height: 1.6;
  }

  a {
    color: #ff66cc;
    text-decoration: none;
  }

  ul {
    padding-left: 1.5rem;
  }

  .fun-facts {
    list-style: "💫 ";
  }
</style>

<div class="container">
  <header>
    <h1>{text}</h1>
    <img src="https://yukiiilove123.github.io/aboutme/Seshomaru.jpg" alt="Cute Avatar" />
  </header>

  <main>
    <h2>✨ about me</h2>
    <p>Hii! I'm Nithya, an 18 y/o from Mumbai 🇮🇳 who adores coding, cute designs, trains 🚆, and languages 🗣️</p>

    <h2>👩🏽‍💻 My KWK Journey</h2>
    <p>Started with KWK’s Data Science camp last year — and I’m back again to keep growing and glowing ✨!</p>

    <h2>🎀 My Passions</h2>
    <p>I love: K-Pop, anime, tech, watching ✨dramas✨, and obsessing over train routes for fun 🚂💖</p>
    <br>
     👉 <a href="https://www.youtube.com/watch?v=3mHbMzBE8Ls&pp=ygUKYXRlZXogd2F2ZQ%3D%3D">here's one of my all time favorite summer kpop songs</a>
    <h2>💖 Fun Facts</h2>
    <ul class="fun-facts">
      <li>Fluent in 5+ languages 🗣️</li>
      <li>Map & geography nerd 🗺️</li>
      <li>Lowkey a train database 🛤️</li>
    </ul>

    <h2>🌐 Connect with me!</h2>
    <p><a href="https://github.com/Yukiiilove123" target="_blank">GitHub 💻</a></p>
    <p><a href="https://www.linkedin.com/in/nithya-anvekar-b578a0283/" target="_blank">LinkedIn 💼</a></p>
  </main>
</div>
