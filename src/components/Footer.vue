<template>
  <footer>
    <nav class="containerf">
      <img alt="Papel-Moeda" id="logo" src="@/assets/logo-Papel-Moeda.png" />
      <div id="Papel-Moeda">
        <span class="papel-moeda">Papel-Moeda</span>
        <span class="up-fin">Upgrade Finaceiro</span>
      </div>
    </nav>
    
  </footer>
</template>

<script>

export default {
  name: "Footer",
}
</script>

<style scoped>
footer {
  width: 100%;
  height: 60px;
  background-color: var(--color-background-nav);
  display: flex;
  justify-content: center;
  align-items: center;
}

#logo {
  width: 56px;
  padding: 5px;
}

.containerf {
  display: flex;
  flex-direction: row;
  align-items: center;
  width: 90%;
}

#Papel-Moeda {
  display: flex;
  flex-direction: column;
  justify-content: start;
}

.up-fin {
  font-family: Ubuntu;
  font-style: normal;
  font-size: 20px;
  line-height: 23px;
  color: #FFFFFF;
}

.papel-moeda {
  font-family: Ubuntu;
  font-style: normal;
  font-weight: bold;
  font-size: 28px;
  line-height: 23px;
  color: #FFFFFF;
}

</style>