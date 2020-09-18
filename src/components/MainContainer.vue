<template>
    <div>
  <p> {{ text }} </p>
  <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Ipsa quae error laboriosam molestias consectetur ipsum maxime natus id delectus, maiores eveniet nesciunt quam, iste commodi dolor? Nemo vero consectetur repudiandae?</p>
 <p> {{ sayi }} </p>
<button @click = art() > Sayı Arttır..</button>
</div>
</template>


<script>
export default {
    data () {
    return {
      text : "loremlorem",
      sayi : 0
    }

  },
  methods : {
      art () {
        this.sayi+=5
      }
      
  },
  computed : {},
  watch : {}
    
}
</script>


<style>

</style>