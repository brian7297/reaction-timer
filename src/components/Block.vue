<template>
  <div class="block">
    click me
  </div>
</template>

<script>
export default {
props: ['delay'],
data() {
    return {
        showBlock: false
    }
},
mounted() {
    console.log('component mounted')
    setTimeout(() => {
        this.showBlock = trueconsole.log(this.delay)
    }, this.delay)
},
updated(){

}
}
</script>

<style>
.Block {
    width: 400px;
    border-radius: 20px;
    color: white;
    text-align: center;
    padding: 100px 0;
    margin: 40px auto;
}
</style>