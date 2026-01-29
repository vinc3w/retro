<script>
  import ReiGif from "$lib/assets/gifs/rei-plushie.gif";
  import AsukaGif from "$lib/assets/gifs/asuka.webp";
  import Asuka2Gif from "$lib/assets/gifs/asuka-2.webp";
  import GayWebsiteGif from "$lib/assets/gifs/gay-website.webp";
  import LoveBrosGif from "$lib/assets/gifs/love-bros.webp";
  import MadeWithVscodeImg from "$lib/assets/imgs/made-with-vscode.png";
  import ResponsiveSiteImg from "$lib/assets/imgs/responsive-site.jpg";
  import { base } from "$app/paths";
</script>

<nav class="container">
  <section>
    <div class="label">♡ navigation ♡</div>
    <ul>
      <li><a href="{base}/">🏠 Home</a></li>
      <li><a href="{base}/gallery">🖼️ Gallery</a></li>
    </ul>
  </section>
  <section>
    <div class="label">♡ Socials ♡</div>
    <ul>
      <li><a href="https://discordapp.com/users/" target="_blank">🖤 Discord</a></li>
      <li><a href="https://www.instagram.com/vinc3w59/" target="_blank">🩷 Instagram</a></li>
      <li><a href="https://open.spotify.com/user/f8sifsire8pgeu635j5n4b2zh?si=c9991214b65f439b" target="_blank">💚 Spotify</a></li>
      <li><a href="https://github.com/vinc3w" target="_blank">💜 Github</a></li>
      <li><a href="https://www.linkedin.com/in/vincent-har/" target="_blank">🩵 LinkedIn</a></li>
    </ul>
  </section>
  <section class="gifs">
    <div class="marquee-gifs">
      <div class="marquee">
        <img src={AsukaGif} alt="asuka gif">
        <img src={Asuka2Gif} alt="asuka 2 gif">
        <img src={GayWebsiteGif} alt="gay wbsite gif">
        <img src={LoveBrosGif} alt="love your bros gif">
        <img src={MadeWithVscodeImg} alt="made with vscode img">
        <img src={ResponsiveSiteImg} alt="responsive site img">
      </div>
    </div>
    <img class="rei-gif" src={ReiGif} alt="rei plushie gif">
  </section>
</nav>

<style>
  nav {
    width: 200px;
    display: flex;
    flex-direction: column;
    gap: 16px;
    padding: 16px 8px;
  }

  .label,
  a {
    border: 1px dashed #000;
    border-radius: 8px;
    padding: 12px 16px;
  }

  .label {
    background-color: #F4ADA0;
  }

  li {
    margin-top: 4px;
  }

  a {
    display: block;
    background-color: #FFC7B8;
  }

  a:hover {
    background-color: #f1bcae;
  }

  section.gifs {
    border: 1px dashed #000;
    border-radius: 8px;
    padding: 8px;
    height: 100%;
  }
  
  .marquee-gifs {
    overflow: hidden;
	}

  .marquee {
    width: fit-content;
		display: flex;
    align-items: center;
		gap: 4px;
    animation: scroll 20s linear infinite;
  }

  .marquee-gifs img {
    height: 40px;
  }

  .rei-gif {
    margin-top: 16px;
    width: 100%;
  }

  @keyframes scroll {
    0% {
      transform: translateX(0);
    }
    50% {
      transform: translateX(calc(-100% + 168px));
    }
    100% {
      transform: translateX(0);
    }
  }
</style>
