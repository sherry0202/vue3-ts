<template>
  <div id="app">
    {{ msg }}
  </div>
  <div>
    <ul>
      <li>1</li>
      <li>2</li>
      <li>3</li>
      <li>4</li>
      <li>5</li>
      <li>6</li>
      <li>7</li>
    </ul>
    <img class="imgLazyLoad" data-src="@/assets/logo.png" alt="图片加载中">
    <ul>
      <li>33</li>
    </ul>
  </div>
  <child v-model:msg="msg"></child>
</template>

<style lang="less">
#app {
  box-sizing: content-box;
  padding: 10px;
  width: 100px;
  height: 100px;
  ul {
    li{
      width: 130px;
      height: 120px;
      background: chocolate;
      margin-top: 10px;
    }

  }
}

</style>
<script>
import Child from "@/child";
export default {
  name: 'app',
  components: {Child},
  data() {
    return {
      msg: 'a2313123',
      imgList : [],
      delay:'',
      time :250,
      offset : 0
    }
  },

  methods:{



  },
}
</script>
