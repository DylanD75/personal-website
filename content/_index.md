+++
title = "Dylan Dehnert"
layout = "home"
url = "/home/"
draft = false
+++

<div style="display: flex; justify-content: center; margin: 30px 0;">
  <img src="/img/dylan_headshot.jpg" 
       alt="Dylan's Headshot" 
       style="border-radius: 50%; width: 250px; height: 250px; object-fit: cover;">
</div>

<div style="text-align: center; margin-top: -25px;">
  <h2>Dylan Dehnert</h2>
</div>

<div style="text-align: center; margin-top: -15px; font-family: 'Nunito Sans', sans-serif; font-size: 1.5rem;">
  <span style="vertical-align: middle;">I am </span>
  <span id="typing" class="typing-text" style="font-weight: bold; vertical-align: middle;"></span>
</div>

<style>
  .social-icons a {
    all: unset;
    display: inline-flex;
    align-items: center;
    justify-content: center;
    cursor: pointer;
  }

  .social-icons a svg {
    display: block;
    margin: 0;
    padding: 0;
    width: 24px;
    height: 24px;
  }

  .social-icons {
    display: flex;
    justify-content: center;
    gap: 15px;
    margin-top: 10px;
  }
</style>

<div class="social-icons">
  <a href="https://www.linkedin.com/in/dylandehnert/" target="_blank" 
     rel="noopener noreferrer me" title="LinkedIn">
    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="none" 
         stroke="currentColor" stroke-width="2" stroke-linecap="round" 
         stroke-linejoin="round">
      <path d="M16 8a6 6 0 016 6v7h-4v-7a2 2 0 00-2-2 2 2 0 00-2 2v7h-4v-7a6 6 0 016-6z"></path>
      <rect x="2" y="9" width="4" height="12"></rect>
      <circle cx="4" cy="4" r="2"></circle>
    </svg>
  </a>
  <a href="https://github.com/DylanD75/" target="_blank" 
     rel="noopener noreferrer me" title="GitHub">
    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="none" 
         stroke="currentColor" stroke-width="2" stroke-linecap="round" 
         stroke-linejoin="round">
      <path d="M 9 19 c -5 1.5 -5 -2.5 -7 -3 m 14 6 v -3.87 a 3.37 3.37 0 0 0 -0.94 -2.61 c 3.14 -0.35 6.44 -1.54 6.44 -7 A 5.44 5.44 0 0 0 20 4.77 A 5.07 5.07 0 0 0 19.91 1 S 18.73 0.65 16 2.48 a 13.38 13.38 0 0 0 -7 0 C 6.27 0.65 5.09 1 5.09 1 A 5.07 5.07 0 0 0 5 4.77 A 5.44 5.44 0 0 0 3.5 8.55 c 0 5.42 3.3 6.61 6.44 7 A 3.37 3.37 0 0 0 9 18.13 V 22"></path>
    </svg>
  </a>
</div>

<style>
  .container {
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
    min-height: 12vh;
    gap: 30px;
  }

  .buttons {
    display: flex;
    justify-content: center;
    gap: 10px;
    margin-left: 10px;
  }

  .button {
    font-size: 15px;
    padding: 8px 16px;
    text-decoration: none;
    border-radius: 8px;
    border: 1px solid currentColor;
    box-shadow: none !important;
  }

  .button:hover {
    background-color: #5c8dd1;
  }
</style>

<div class="container">
  <div class="buttons">
    <a class="button" href="/about/" rel="noopener" title="About">
      <span class="button-inner"><b>About</b></span>
    </a>
    <a class="button" href="/projects/" rel="noopener" title="Projects">
      <span class="button-inner"><b>Projects</b></span>
    </a>
    <a class="button" href="/resume/" rel="noopener" title="Resume">
      <span class="button-inner"><b>Resume</b></span>
    </a>
  </div>
</div>


<style>
  .typing-text {
    white-space: nowrap;
    overflow: hidden;
    border-right: 2px solid black;
    display: inline-block;
    animation: blink-cursor 0.8s steps(2) infinite;
  }

  @keyframes blink-cursor {
    0%, 100% { border-color: transparent; }
    50% { border-color: #555555; }
  }
</style>

<script>
  const textElement = document.getElementById("typing");
  const words = ["a CS and Statistics student.", "an aspiring software engineer/trader.", "a problem solver.", "a calculated risk-taker.", "a curious learner.", "excited to connect with you!"];
  let wordIndex = 0;
  let letterIndex = 0;
  let isDeleting = false;

  function typeWords() {
    const currentWord = words[wordIndex];

    if (isDeleting) {
      letterIndex--;
    } else {
      letterIndex++;
    }

    textElement.textContent = currentWord.substring(0, letterIndex);

    let typingSpeed = isDeleting ? 50 : 100;

    if (!isDeleting && letterIndex === currentWord.length) {
      typingSpeed = 1000;
      isDeleting = true;
    } else if (isDeleting && letterIndex === 0) {
      isDeleting = false;
      wordIndex = (wordIndex + 1) % words.length;
      typingSpeed = 500;
    }

    setTimeout(typeWords, typingSpeed);
  }

  document.addEventListener("DOMContentLoaded", typeWords);
</script>