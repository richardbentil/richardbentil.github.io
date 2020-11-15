<template>
  <div>
    <main>
      <div class="row my-4 py-5">
        <div class="col-md-6">
          <div class="card shadow border-0">
            <div class="card-body text-center">
              <figure>
                <img class="rounded-circle mx-auto py-3 pb-3" width="200" src="avatar.jpg" alt="profile picture of Richard Bentil">
                <figcaption>
                  <h2 class="card-title">Richard Bentil</h2>
                  <h3 class="card-text font-weight-normal py-3 pb-5">Web Developer</h3>
                </figcaption>
              </figure>
            </div>
            <div class="card-footer text-center">
                <router-link to="https://www.linkedin.com/in/richard-bentil-636051115" target="_blank">
                <i class="fa fa-linkedin fa-lg p-2" aria-hidden="true"></i>
                </router-link>
                <router-link to="https://web.facebook.com/bricks.murphy" target="_blank">
                <i class="fa fa-facebook fa-lg p-2" aria-hidden="true"></i>
                </router-link>
            </div>
          </div>
        </div>
        <article class="col-md-6">
                  <h1>Hi</h1>
                  <p>I'm Richard, a Web Developer based in Accra, Ghana.</p>
                  <p>I enjoy developing responsive functional websites using <b>React JS</b> and <b>Vue JS</b>. Moreover I work with <b>PHP</b> and <b>MySQL</b> to store data. I also develop WordPress themes.</p>
                  <div class="my-5">
                    <router-link class="btn btn-primary btn-md mr-2" to="/projects">Projects</router-link>
                    <router-link class="btn btn-outline-primary btn-md" to="/resume">Resume</router-link>
                  </div>
           </article>
        </div>
      </main>
  </div>
</template>