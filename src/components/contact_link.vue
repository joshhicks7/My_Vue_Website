<template>
    <div class="contact_link">
        <img v-if="img" :src= "img"/>
        <a :href = "link" target = "blank">{{title}}</a>
    </div>
</template>

<script>

export default
{
    name:'contact_link',
   props:
   {
       link:String,
       title:String,
       img:String
   }
}
</script>

<style lang="postcss" scoped>
    img
    {
        width:25px;
    }
    .contact_link
    {
        font-size: 25px;
    }
</style>
