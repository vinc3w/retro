<script>
  import SideBar from "./SideBar.svelte";
  import WelcomeGif from "$lib/assets/gifs/welcome-blinks.gif";
  import AsukaGif from "$lib/assets/gifs/asuka.gif";
  import NinoShyGif from "$lib/assets/gifs/nino-shy.gif";
  import NatureGif from "$lib/assets/gifs/nature.gif";
  import EnterButtonGif from "$lib/assets/gifs/enter-button.gif";
</script>

<div class="main-content">
  <div class="container">
    <div class="row">
      <img src={WelcomeGif} alt="welcome gif">
      <div>
        This is where I get to show off my personality 🤪 — I hope you don't mind. Hehe 😭
      </div>
    </div>
    <div class="row">
      <div>
        Harrow 👋 My name is Vincent, a 2005 kid, gamer ⌨️, programmer 🧑‍💻, and honestly… many more things. More specifically, I’m a Full-Stack Web Developer 🤪, which means I handle both the pretty ✨ stuff you see on a website and the logic behind it — servers 🎮, databases, and all that technical magic. I also really enjoy designing 💜 things (this website is literally the result of that).
      </div>
    </div>
    <div class="row">
      <div>
        Here, I try to include my hobbies, likes, and maybe even a few dislikes ⁉️ Yeah… I’m still figuring out what to put sometimes 🥺 But anyway, feel free to look around 👀, maybe give me a follow on my socials, and most importantly — enjoy your stay ✨
      </div>
      <img src={AsukaGif} alt="asuke gif">
    </div>
  </div>
  <div class="content-row">
    <a href="https://vinc3w.github.io/" target="_blank" class="portfolio">
      <img src={NatureGif} alt="nature background" class="bg">
      <div class="content">
        Visit my professional portfolio
        <img src={EnterButtonGif} alt="enter button gif">
      </div>
    </a>
    <img class="nino" src={NinoShyGif} alt="shy nino gif">
  </div>
</div>
<SideBar />

<style>
  .main-content {
    display: flex;
    gap: 4px;
    flex-direction: column;
    width: 100%;
  }

  .container {
    width: 100%;
    height: 100%;
    text-align: center;
    padding: 16px;
    display: flex;
    flex-direction: column;
    gap: 32px;
  }

  .container .row {
    display: flex;
    align-items: center;
    gap: 16px;
  }

  .container .row > * {
    width: 100%;
  }

  .content-row {
    display: flex;
    gap: 4px;
    height: 250px;
  }

  .portfolio img.bg,
  img.nino {
    border-radius: 8px;
    border: 1px solid #000;
  }

  .portfolio {
    width: 100%;
    position: relative
  }

  .portfolio img.bg {
    height: 100%;
    width: 100%;
  }

  .portfolio .content {
    position: absolute;
    top: 0;
    left: 0;
    height: 100%;
    width: 100%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    color: #FFF;
    font-size: 18px;
  }

  .portfolio .content img {
    margin-top: 12px;
  }
</style>
