---
layout: page
title: About
permalink: /about/
---

<div class="about-container">
  <img src="/assets/img/profile.png" alt="Om Biradar" class="profile-photo">
  
  <div class="about-text">
    <p>
        Hi, I'm <strong>Om Biradar</strong>.
    </p>
    <p>
        I'm a programmer. I do things that interest me.
    </p>
    <p>
        I am also an upcoming SDE at NatWest Group.
    </p>
    <p>
        This blog is my personal space to write notes, explanations, experiments, and thoughts.
    </p>
    <p>
        Feel free to reach out if you want to discuss, share ideas, or just say hi.
    </p>

    Thanks for visiting!
  </div>
</div>

<style>
  .about-container {
    display: flex;
    flex-wrap: wrap;
    gap: 30px;
    align-items: flex-start;
    margin-bottom: 2rem;
  }

  .profile-photo {
    width: 300px;
    max-width: 50%;
    height: auto;
    border-radius: 50%;
    object-fit: cover;
  }

  .about-text {
    flex: 1;
    min-width: 300px;
  }

  /* Mobile / narrow screens */
  @media (max-width: 599px) {
    .about-container {
      flex-direction: column;
      align-items: center;
      text-align: center;
    }

    .profile-photo {
      max-width: 300px;
      width: 100%;
      margin: 0 auto 1.5rem;
    }

    .about-text {
      text-align: left;
    }
  }
</style>
