<template>
  <div>
    <div class="row">
        <div class="col">StyleCode</div>
        <div class="col">Description</div>
        <div class="col">Active</div>
        <div class="col">Background Image</div>
        <div class="col">Message Length Limit</div>
        <div class="col">Message Line Limit</div>
    </div>
    <div class="row" v-for="item in stylecodes" :key="item.stylecode">
        <div class="col">{{item.stylecode}}</div>
        <div class="col">{{item.styledescription}}</div>
        <div class="col">{{item.active}}</div>
        <div class="col">{{item.backgroundimage}}</div>
        <div class="col">{{item.messagelengthlimit}}</div>
        <div class="col">{{item.messagelinelimit}}</div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'StyleCodeAll',
  /*
  props: {
    stylecodes: Object
  },
  */
  data() {
      return {
          stylecodes: [
              {stylecode:"AAA", styledescription:"this is what it is", styleactive: true, stylebackgroundimage: "image.png", messagelengthlimit: 500, messagelinelimit: 8},
              {stylecode:"BBB", styledescription:"this is what it is", styleactive: true, stylebackgroundimage: "image.png", messagelengthlimit: 500, messagelinelimit: 8},
              {stylecode:"CCC", styledescription:"this is what it is", styleactive: true, stylebackgroundimage: "image.png", messagelengthlimit: 500, messagelinelimit: 8},
              {stylecode:"DDD", styledescription:"this is what it is", styleactive: true, stylebackgroundimage: "image.png", messagelengthlimit: 500, messagelinelimit: 8},
            ]
      }
      
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
