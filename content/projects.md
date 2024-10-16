+++
title = "Projects"
layout = "projects"
url = "/projects/"
summary = "Projects"
+++

<h3>Summary 📋</h3>

Here is a collection of the projects and cool things I have worked on. Ranging from personal programs to school projects, this portfolio adequately displays my passions and skills. Feel free to contact me with any questions or comments about my work.

<style>
  .gallery {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 30px;
    padding: 0px;
    margin-top: 30px;
  }

  @media (max-width: 650px) {
    .gallery {
      grid-template-columns: 1fr;
      justify-items: center;
    }
  }

  .project-card {
    aspect-ratio: 1 / 1;
    width: 100%;
    max-width: 600px;
    border: 2.5px solid currentColor;
    border-radius: 8px;
    overflow: hidden;
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center;
    box-shadow: none !important;
    background-color: var(--theme);
    cursor: pointer;
    text-decoration: none;
    color: inherit;
  }

  .project-card img {
    width: 100%;
    height: auto;
    object-fit: cover;
    margin: 0;
  }

  .project-card h3 {
    margin-top: 8px;
    font-size: 16px;
  }

  .project-card p {
    padding: 0 10px 15px;
    margin-top: -13px;
    font-size: 12px;
  }

  @media (max-width: 708px) {
    .project-card h3 {
      font-size: 14px;
      margin-top: 9px;
    }

    .project-card p {
      font-size: 10px;
      margin-top: -13px;
    }
  }

  @media (max-width: 650px) {
    .project-card h3 {
      font-size: 25px;
      margin-top: 10px;
    }

    .project-card p {
      font-size: 15px;
      margin-top: -6px;
    }
  }
</style>

<div class="gallery">
  <a href="https://github.com/DylanD75/poker-bot" class="project-card">
    <img src="/img/poker-bot-pic.png" alt="PokerBot Image">
    <h3>PokerBot</h3>
    <p>This AI PokerBot, named "Jester," plays heads-up poker against a user player, utilizing an unexploitable GTO-style strategy. Test your poker skills and see if you can beat Jester!</p>
  </a>

  <a href="https://github.com/DylanD75/RocketRob" class="project-card">
    <img src="/img/rocketrob-pic.png" alt="Lotka Volterra Image">
    <h3>RocketRob</h3>
    <p>RocketRob is a Unity game on the IOS App Store from Aphy Games. The game is a pixelated 2D platformer that depicts a character named Rob launching as high as possible with his rocket launcher!</p>
  </a>

  <a href="https://github.com/DylanD75/lotka-volterra-simulation" class="project-card">
    <img src="/img/lotka-volterra-pic.png" alt="Lotka Volterra Image">
    <h3>Lotka Volterra Simulation</h3>
    <p>The Lotka Volterra Simulation is a Unity project that models the relationship between predator and prey populations through a visual simulation. This was the final project for my AP Calculus AB class.</p>
  </a>
</div>

<style>
  .more-projects-text {
    text-align: center;
    margin-top: 30px;
    font-size: 18px;
  }
</style>

<p class="more-projects-text">
  ...more projects to be added soon 😁
</p>