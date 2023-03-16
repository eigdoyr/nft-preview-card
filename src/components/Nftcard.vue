<template>
  <div class="card-container">
    <div class="img-container">
      <a href="#">
        <img
          class="main-img"
          src="../assets/image-equilibrium.jpg"
          alt="Equilibrium image"
        />
      </a>
      <div class="img-overlay"></div>
    </div>
    <div class="main-title">
      <h1 class="main-heading"><a href="#">Equilibrium #3429</a></h1>
      <p class="main-leading">
        Our Equilibrium collection promotes balance and calm.
      </p>
    </div>
    <div class="token-details">
      <span class="token">0.041 ETH</span>
      <span class="token-days-left">3 days left</span>
    </div>
    <hr />
    <div class="creator-details">
      <img
        class="creator-icon"
        src="../assets/image-avatar.png"
        alt="creator image"
      />
      <h2 class="creator">
        Creation of <a href="#" class="creator-name">Jules Wyvern</a>
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
  color: var(--cyan);
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
  transition: 0.3s ease;
  background-color: hsla(178, 100%, 50%, 0.5);
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

.main-heading {
  font-size: 1.5rem;
  padding: 1rem 0;
}

.main-leading {
  color: var(--soft-blue);
  padding: 0.2rem 0;
  font-weight: 300;
  line-height: 1.5rem;
  font-size: 1.1rem;
}

.token-details {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  padding: 1rem 0;
  align-self: center;
}

.token {
  color: var(--cyan);
  font-weight: 600;
}

.token:before {
  content: url("../assets//icon-ethereum.svg");
  margin-right: 0.5rem;
  position: relative;
  top: 3px;
}

.token-days-left {
  color: var(--soft-blue);
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

.creator {
  font-size: 1rem;
  color: var(--soft-blue);
  font-weight: 400;
  padding-left: 1rem;
}

.creator-details {
  display: flex;
  align-items: center;
  padding: 0.25rem 0;
}

@media (width>=845px) {
  .main-heading a {
    font-size: 1.345rem;
  }
}
</style>
