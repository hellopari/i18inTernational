<template>
<div>
<div class="lang">
    <div>{{ $t("message.Username") }}</div>
</div>

<button @click="changLang('en')">切换成英文</button>
<button @click="changLang('zh')">切换成中文</button>
</div>

</template>

<script>
export default {

  name: 'HelloWorld',
  methods:{
    changLang(lan){
        this.$i18n.locale = lan;
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
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
