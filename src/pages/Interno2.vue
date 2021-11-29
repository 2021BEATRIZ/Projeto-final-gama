<template>
  <main>
    <section class="container">
      <div class="container">
        <div class="resumo">
          <h1>Poupando e rendendo</h1>
          <span
            >Sed ut perspiciatis unde omnis iste natus error sit voluptatem
            accusantium doloremque laudantium, totam rem aperiam, eaque ipsa
            quae ab illo inventore veritatis et quasi architecto beatae vitae
            dicta sunt explicabo. Nemo enim ipsam voluptatem quia voluptas sit
            aspernatur aut odit aut fugit, sed quia consequuntur magni dolores
            eos qui ratione voluptatem sequi nesciunt.
          </span>
        </div>
        <div class="resumo">
          <img alt="" id="logoCurso" src="@/assets/bolinha8.png" />
        </div>
      </div>
    </section>
    
  </main>
</template>

<script>
import api from "@/services/api.js";

export default {
  name: "Interno2",
  data() {
    return {
      videos: [],
    };
  },
  mounted() {
    api.get("/videos.json").then((response) => {
      this.videos = response.data;
    });
  },
};
</script>

<style scoped>
main {
  margin: 3%;
}

#logoCurso {
  width: 65%;
}

.resumo {
  float: left;
  width: 30%;
  margin-bottom: 2%;
}


</style>