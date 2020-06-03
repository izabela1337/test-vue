<template>
    <div class="container">
        <buttonq></buttonq>
        <button @click="$refs.slider.next()">next</button>
        <ReaderSlider :options="options" ref="slider" :items="items">
            <template v-slot:item="{ item, index, active }">
                <ReaderItem :index="index" :active="active">
                    <img :src="item.src"/>
                    <p>Strona: {{ index + 1 }}</p>
                </ReaderItem>
             </template>
            <template v-slot:pagination="{ item, current, total }">
                <ReaderPagination :current="current" :total="total">
                    <div> {{ current + '/' + total }} </div>
                </ReaderPagination>
            </template>
    </ReaderSlider>
    </div>
</template>
 
<script>
    import button123 from "@/components/button123.vue";
    export default {
        name: "Home",
        components: {
        "buttonq": button123
         },
        data () {
        const items = []
        for (let i = 1; i <= 9; i++) {
        items.push({ src: `/manga/3/00${i}.jpg` })
        }
        return {
        items,
        options: {
           width: "90%",
           height: "90%",
           direction: "vertical",
           virtual: false
        }
        }
    },
    methods: {
    submit(){
      this.counter++;
      console.log(this.ref)
    }
    }
    }
</script> 
 
<style lang="scss" scoped>
img{
    max-height: 100%;
    max-width: 100%;
}
</style>