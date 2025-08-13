<template>
  <div class="before_quantity">
        <form>
          <p>
            <label class="people" for="people_num"><input type="" class="people" id="people_num" />人分</label>
          </p>
          <p class="quanity_1_name_p">
            <label class="quanity_name quanity_1_name" for="quanity_1_name_input">材料名<input type="text" class="quanity_name quanity_1_name" id="quanity_1_name_input" /></label>
            <label class="quanity quanity_1" for="quanity_1_input">分量<input type="number" class="quanity quanity_1" id="quanity_1_input" /></label>
            <label class="unit unit_name" for="unit_1_input">単位<select class="unit_select" id=" unit_1_input"><option value="">単位を選択してください</option><option value="g">g</option><option value="ml">ml</option><option value="cc">cc</option><option value="大さじ">大さじ</option><option value="小さじ">小さじ</option><option value="カップ">カップ</option><option value="合">合</option><option value="g">個</option></select></label>
          </p>
          <button type="button" class="quanity_increase">材料を増やす</button>
          <button type="button" class="quanity_completed">入力終了</button>
        </form>
  </div>
</template>

<script lang="ts">
import { Options, Vue } from 'vue-class-component'

@Options({
  props: {
    msg: String
  }
})
export default class HelloWorld extends Vue {
  msg!: string
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
