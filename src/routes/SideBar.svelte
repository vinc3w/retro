<script>
  import ComputerGeekGif from "$lib/assets/gifs/100-computer-geek.webp";
  import HeavilyMedicatedGif from "$lib/assets/gifs/heavily-medicated.gif";
  import ComputerLoveGif from "$lib/assets/gifs/i-love-my-computer.gif";
  import RealLifeAngelGif from "$lib/assets/gifs/real-life-angel.webp";
  import TransRightGif from "$lib/assets/gifs/transrights.gif";
  import DownRightArrow from "$lib/assets/icon/DownRightArrow.svelte";
  import Avatar from "$lib/assets/imgs/avatar.png";
</script>

<div class="container info">
  <div class="label">♡ Notes ♡</div>
  <section class="notes">
    <ul>
      <li>he / him</li>
      <li>cis male</li>
      <li>straight</li>
      <li>sagittarius</li>
      <li>ISFP</li>
    </ul>
  </section>
  <section class="gifs">
    <img src={ComputerGeekGif} alt="computer geek gif">
    <img src={HeavilyMedicatedGif} alt="heavily medicated gif">
    <img src={ComputerLoveGif} alt="i love my computer gif">
    <img src={RealLifeAngelGif} alt="real life angel gif">
    <img src={TransRightGif} alt="trans rights gif">
  </section>
  <a class="avatar" href="https://www.roblox.com/users/2289176113/profile" target="_blank">
    <img src={Avatar} alt="roblox avatar">
    <div class="indicator">
      <DownRightArrow />
      <div>
        Follow me <br/>
        on Roblox!
      </div>
    </div>
  </a>
  <div class="label visitor-label">♡ Visitors ♡</div>
  <div class="counter">
    <script language="javascript" type="text/javascript" src="//counter1.fc2.com/counter.php?id=40706216&main=1"></script>
    <noscript>
      <img src="//counter1.fc2.com/counter_img.php?id=40706216&main=1" alt="counter" />
    </noscript>
  </div>
</div>

<style>
  .info {
    padding: 16px 8px;
    min-width: 250px;
    max-width: 250px;
  }

  section.notes {
    border: 1px dashed #000;
    padding: 8px;
    margin-top: 8px;
    border-radius: 8px;
  }

  section.notes li {
    list-style-type: disc;
    list-style-position: inside;
  }

  section.gifs {
    margin-top: 16px;
  }

  section.gifs img {
    width: 100%;
    display: block;
  }

  a.avatar {
    display: block;
  }

  a.avatar img {
    width: 100%;
  }

  a.avatar .indicator {
    display: flex;
    align-items: center;
    justify-content: flex-end;
    gap: 16px;
    padding-right: 24px;
  }

  .visitor-label {
    margin-top: 16px;
  }

  .counter {
    margin-top: 16px;
  }

  .label{
    border: 1px dashed #000;
    border-radius: 8px;
    padding: 12px 16px;
    background-color: #F4ADA0;
  }
</style>
