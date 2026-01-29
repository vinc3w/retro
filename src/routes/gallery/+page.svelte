<script>
  import img2 from "$lib/assets/imgs/gallery/gallery-img-2.jpeg";
  import img4 from "$lib/assets/imgs/gallery/gallery-img-4.jpeg";
  import img5 from "$lib/assets/imgs/gallery/gallery-img-5.jpeg";
  import img6 from "$lib/assets/imgs/gallery/gallery-img-6.jpeg";
  import img7 from "$lib/assets/imgs/gallery/gallery-img-7.jpeg";
  import img8 from "$lib/assets/imgs/gallery/gallery-img-8.jpeg";
</script>

<div class="container">
  <div class="text">
    <div class="title">
      Welcome to my little corner of the internet ✨🖼️
    </div>
    <div class="intro">
      This gallery is a scrapbook of experiments, memories, and random sparks of creativity I've collected along the way 🌱💡 From pixel art and sketches to screenshots of projects I'm proud of, every image here tells a tiny story 📸💭 Feel free to wander, click around, and get lost in the vibes — this space is meant to be playful, personal, and a bit nostalgic 💾🌈 Thanks for stopping by and sharing this moment with me 💖
    </div>
  </div>
  <div class="images">
    <div class="col col-1">
      <div class="img-container"><img src={img4} alt="gallery 4"></div>
      <div class="img-container"><img src={img2} alt="gallery 2"></div>
    </div>
    <div class="col col-2">
      <div class="img-container"><img src={img7} alt="gallery 7"></div>
      <div class="img-container"><img src={img8} alt="gallery 8"></div>
      <div class="img-container"><img src={img5} alt="gallery 5"></div>
      <div class="img-container"><img src={img6} alt="gallery 6"></div>
    </div>
  </div>
</div>

<style>
  .container {
    width: 100%;
    text-align: center;
    padding: 8px;
  }

  .text {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    gap: 32px;
    padding: 64px;
  }

  .title {
    font-size: 24px;
  }

  .images {
    display: flex;
    gap: 4px;
  }

  .col {
    width: 100%;
    display: flex;
    flex-direction: column;
    gap: 4px;
  }

  .img-container {
    padding: 4px;
    background-color: #FFF;
    border-radius: 8px;
    border: 1px solid #000;
  }
  
  img {
    display: block;
    width: 100%;
    border-radius: 8px;
  }
</style>
