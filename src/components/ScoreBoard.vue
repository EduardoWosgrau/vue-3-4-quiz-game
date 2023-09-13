<template>
  <div class="hello">
    <section class="score">
      Player <span> {{ this.winCount }}</span> x Computer <span>{{ this.loseCount }}</span>
    </section>
  </div>
</template>

<script>
export default {
  name: 'ScoreBoard',
  props: ['winCount', 'loseCount']
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  section.score {
    border-bottom: 1px solid black;
    padding: 24px;
    font-size: 18px;
   
    span{
      padding: 8px;
      font-weight: bold;
      border: 1px solid black;
    }
  }
</style>
