<template>
  <div id="secondcomponent">
    <h1>I am another page</h1>
    <a> written by {{ author }} </a>
    <p> 感谢 <a href="https://github.com/showonne">showonne</a>大神的技术指导</p>
    <ul id="example-2">
    <li v-for="(item, index) in articles">
      {{ index }} - {{ item.message }}
    </li>
  </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      author: "微信公众号 jinkey-love",
      articles: [
          { message: 'Foo' },
          { message: 'Bar' }
      ],
    }
  }
}
</script>

<style>
</style>