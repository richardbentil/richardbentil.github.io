<template>
  <div>
    <header>
  <nav class="navbar navbar-expand-sm navbar-light py-4" style="background-color: rgb(255, 255, 255);">
      <div class="container">
      <router-link class="navbar-brand" to="/">
        <img src="small_logo.png" width="30" alt="logo">
      </router-link>
      <button class="navbar-toggler d-lg-none" type="button" data-toggle="collapse" data-target="#collapsibleNavId" aria-controls="collapsibleNavId"
          aria-expanded="false" aria-label="Toggle navigation"></button>
      <div class="collapse navbar-collapse" id="collapsibleNavId">
          <ul class="navbar-nav ml-auto mt-2 mt-lg-0">
          <li class="nav-item">
            <router-link class="nav-link active" to="/">About me <span class="sr-only">(current)</span>
            </router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/projects">Projects
            </router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/resume">Resume</router-link>
            </li>
          <li class="nav-item"><router-link class="nav-link" to="/contact">Contact</router-link>
          </li>
          </ul>
      </div>
      </div>
  </nav>
  </header>
  </div>
</template>

<script>
export default {
  name: "Navigation",
};
</script>
