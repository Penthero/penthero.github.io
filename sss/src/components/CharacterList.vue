<template>
  <div class="character-list">
    <router-link :to="{name: 'character-profile', params: {character: 'sofia'}}">
      <div class="character-portrait sofia"></div>
    </router-link>
    <router-link :to="{name: 'character-profile', params: {character: 'alith'}}">
      <div class="character-portrait alith"></div>
    </router-link>
    <router-link :to="{name: 'character-profile', params: {character: 'pareth'}}">
      <div class="character-portrait pareth"></div>
    </router-link>
    <router-link :to="{name: 'mornn-profile'}">
      <div class="character-portrait mornn"></div>
    </router-link>
  </div>
</template>

<style lang="scss" scoped>
.character-list {
  width: 120px;
  display: flex;
  align-items: center;
  flex-direction: column;
  margin-right: 20px;
  margin-top: -5px;
}

.character-portrait {
  width: 140px;
  height: 180px;
  margin: 10px;
  text-align: center;
  background-size: cover;
  transition: all 300ms;

  &.sofia {
    background-image: url("../assets/images/sofia-portrait.png");
  }

  &.alith {
    background-image: url("../assets/images/alith-portrait.png");
  }

  &.pareth {
    background-image: url("../assets/images/pareth-portrait.png");
  }

  &.mornn {
    background-image: url("../assets/images/mornn-portrait.png");
    height: 140px;
  }
}
</style>