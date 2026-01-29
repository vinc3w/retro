<script>
  import Nino1 from "$lib/assets/imgs/nino-expressions/nino-1.png";
  import Nino2 from "$lib/assets/imgs/nino-expressions/nino-2.png";
  import Nino3 from "$lib/assets/imgs/nino-expressions/nino-3.png";
  import Nino4 from "$lib/assets/imgs/nino-expressions/nino-4.png";
  import Nino5 from "$lib/assets/imgs/nino-expressions/nino-5.png";
  import Nino6 from "$lib/assets/imgs/nino-expressions/nino-6.png";
  import Nino7 from "$lib/assets/imgs/nino-expressions/nino-7.png";
  import Nino8 from "$lib/assets/imgs/nino-expressions/nino-8.png";
  import Nino9 from "$lib/assets/imgs/nino-expressions/nino-9.png";
  import Nino10 from "$lib/assets/imgs/nino-expressions/nino-10.png";
  import Nino11 from "$lib/assets/imgs/nino-expressions/nino-11.png";
  import Nino12 from "$lib/assets/imgs/nino-expressions/nino-12.png";

  const ninoImages = [
    Nino1, Nino2, Nino3, Nino4, Nino5, Nino6,
    Nino7, Nino8, Nino9, Nino10, Nino11, Nino12
  ];
</script>

<div class="welcome-marquee container">
  <div class="marquee">
    {#each ninoImages as ninoImg, i}
      {#if i !== ninoImages.length}
        <div class="item">WELCOME TO MY DIGITAL SPACE</div>
        <div class="item">
          <img src={ninoImg} alt="Nino Expression" />
        </div>
      {:else}
        <div class="item">
          <img src={ninoImg} alt="Nino Expression" />
        </div>
        <div class="item">WELCOME TO MY DIGITAL SPACE</div>
      {/if}
    {/each}
  </div>
</div>

<style>
	.welcome-marquee {
		height: 70px;
		margin-top: 4px;
    overflow: hidden;
	}

  .marquee {
    height: 100%;
		display: flex;
    align-items: center;
		gap: 32px;
    padding: 0 32px;
    animation: scroll 30s linear infinite;
  }

  .item {
    white-space: nowrap;
  }

  img {
    height: 25px;
  }

  @keyframes scroll {
    0% {
      transform: translateX(0);
    }
    50% {
      transform: translateX(-100%);
    }
    100% {
      transform: translateX(0);
    }
  }
</style>