<template>
    <div>
        <div class="row py-5">
            <div class="col-12">
                <section>
                <h3 class="text-center my-3">Projects</h3>
                <article v-for="project in projects" :key="project.index" class="card shadow border-0 my-md-5 my-sm-3 my-2">
                    <div class="card-body">
                        <div class="media mt-5 mx-md-4 mx-sm-3 mx-2">
                            <div class="media-body">
                                <h4 class="text-primary mb-3">{{ project.name }}</h4>
                                <router-link class="btn btn-primary btn-sm mr-2"  :to="project.link" target="_blank">View Project</router-link>
                                <router-link class="btn btn-outline-primary btn-sm"  :to="project.githublink" target="_blank">Github</router-link>
                                <div class="mt-4">
                                    <p class="font-weight-bold">Description</p>
                                    <p class="mt-n2">{{ project.description }}</p>
                                    <p class="font-weight-bold">Technologies</p>
                                    <p class="mt-n2">{{ project.technologies }}</p>
                                </div>
                            </div>
                        </div>
                    </div>
            </article>
            </section>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    name: "Projects",
    data: function() {
        return {
            projects :[
                {
                    name: "Simpleclass",
                    description: `A web app to help tutors upload course materials to help students 
                     have access to them`,
                    link: "/simpleclass",
                    githublink: "https://github.com/richardbentil/simpleclass",
                    "technologies": "PHP, SQL"
                },
                
                {
                    name: "Asteroids in space",
                    description: `A web app showing the number of asteroids in space.
                     Axios is used to fetch these asteroids from the NASA API.`,
                 
                    link: "/space",
                    githublink: "https://github.com/richardbentil/space",
                    technologies: "Vue, Axios, NASA API"
                },
                {
                    name: "City Guide",
                    description: `A webiste showing the city of Accra. 
                     This page showcases my basic web design skills.`,
                    link: "/city-guide",
                    githublink: "https://github.com/richardbentil/city-guide",
                    technologies: "HTML, CSS"
                }
            ]
        }
    }
}
</script>

