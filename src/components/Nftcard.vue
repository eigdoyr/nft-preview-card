<template>
  <div class="card-container">
    <div class="img-container">
      <a href="#">
        <img
          class="main-img"
          src="../assets/bored-ape8921.jpeg"
          alt="Equilibrium image"
        />
      </a>
      <div class="img-overlay"></div>
    </div>
    <div class="main-title">
      <h1 class="main-heading">
        <a
          href="https://opensea.io/assets/ethereum/0xbc4ca0eda7647a8ab7c2061c2e118a18a936f13d/8921"
          target="_blank"
          >Bored APE #8921</a
        >
      </h1>
      <p class="main-leading">
        <!-- Our Equilibrium collection promotes balance and calm. -->
        Cartoon of ape that is procedurally generated by an algorithm.
      </p>
    </div>
    <div class="token-details">
      <span class="token">5.01 ETH</span>
      <span class="token-days-left">2 days left</span>
    </div>
    <hr />
    <div class="creator-details">
      <img
        class="creator-icon"
        src="https://i.seadn.io/gae/-5WaVFmGTsADRQpwQNheyS8LSH4LcKQMrQC3xDPFEnpkfr5rQ7y4Fj0jyGiqX4jU69TSXFDo2MN4uv_1vtlwIc_k_2c3LsOdNAa8Tw?auto=format&w=1000"
        alt="creator image"
      />
      <h2 class="creator">
        Creation of
        <a href="https://yuga.com" target="_blank" class="creator-name"
          >Yuga Labs</a
        >
      </h2>
    </div>
  </div>
</template>

<style scoped>
img {
  width: 100%;
  height: auto;
}

hr {
  background-color: var(--line);
  border: none;
  height: 1px;
  margin-bottom: 1rem;
}

a {
  text-decoration: none;
  color: var(--white);
}

a:hover {
  color: var(--primary);
}

.main-img {
  border-radius: 10px;
  display: block;
  height: auto;
}

.img-container {
  position: relative;
}

.img-overlay:hover,
.img-container {
  opacity: 1;
}

.img-overlay {
  background-image: url("../assets/icon-view.svg");
  background-position: center;
  background-repeat: no-repeat;
  position: absolute;
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
  opacity: 0;
  -webkit-transition: 0.3s ease;
  -o-transition: 0.3s ease;
  transition: 0.3s ease;
  background-color: hsla(66, 73%, 63%, 0.5);
  /* background-color: hsla(178, 100%, 50%, 0.5); */
  border-radius: 10px;
  cursor: pointer;
}

.card-container {
  background-color: var(--card-bg);
  padding: 1.5rem;
  margin: 1.5rem;
  border-radius: 1em;
  max-width: 22.125rem;
}

.card-container {
  -webkit-transition: all 0.5s ease;
  -o-transition: all 0.5s ease;
  transition: all 0.5s ease;
  /* box-shadow: 0 0 1px #fff, 0 0 10px #fff, 0 0 12px #fff, 0 0 2px #01f7ff,
    0 0 8px #01f7ff, 0 0 10px #01f7ff, 0 0 10px #01f7ff, 0 0 160px #01f7ff; */
}
/* .card-container:hover {
  background: linear-gradient(
    280deg,
    rgba(38, 54, 54, 1) 0%,
    rgba(35, 35, 69, 1) 48%,
    rgb(24, 115, 133) 100%
  );
  transition: all 0.3s ease;
  box-shadow: 0 0 1px #fff, 0 0 10px #fff, 0 0 5px #fff, 0 0 2px #01f7ff,
    0 0 8px #01f7ff, 0 0 5px #01f7ff, 0 0 5px #01f7ff, 0 0 0px #01f7ff;
} */

.main-heading {
  font-size: 1.5rem;
  padding: 1rem 0;
}

.main-leading {
  color: var(--soft-yellow);
  padding: 0.2rem 0;
  font-weight: 300;
  line-height: 1.5rem;
  font-size: 1.1rem;
}

.token-details {
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-orient: horizontal;
  -webkit-box-direction: normal;
  -ms-flex-direction: row;
  flex-direction: row;
  -webkit-box-pack: justify;
  -ms-flex-pack: justify;
  justify-content: space-between;
  padding: 1rem 0;
  -ms-flex-item-align: center;
  -ms-grid-row-align: center;
  align-self: center;
}

.token {
  color: var(--primary);
  font-weight: 600;
}

.token:before {
  content: url("../assets//icon-ethereum.svg");
  margin-right: 0.5rem;
  position: relative;
  top: 3px;
}

.token-days-left {
  color: var(--soft-yellow);
}

.token-days-left:before {
  content: url("../assets/icon-clock.svg");
  margin-right: 0.5rem;
  position: relative;
  top: 3px;
}

.creator-icon {
  width: 36px;
  border: 2px solid var(--white);
  border-radius: 50px;
}

.creator-icon:hover {
  border-color: rgb(103, 103, 245);
}
.creator {
  font-size: 1rem;
  color: var(--soft-yellow);
  font-weight: 400;
  padding-left: 1rem;
}

.creator-details {
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-align: center;
  -ms-flex-align: center;
  align-items: center;
  padding: 0.25rem 0;
}

@media (width>=845px) {
  .main-heading a {
    font-size: 1.345rem;
  }
}
</style>
