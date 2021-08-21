<template>   
    <a :href = "link" class="project">        
        <h2 class="project_title" >{{title}}</h2>
        <p class="project_description">{{description}}</p>
        <img  v-if='image' class="project_image" :src= "img"/>  
    </a>
</template>

<script>
    export default
    {
        name:'Project',
        props:
        {
            img:String,
            title:String,
            description:String,
            link:String
        }
    }
</script>

<style scoped>
    a
    {
        width:fit-content;
        height:fit-content;
        text-decoration:none;
    }
    .project
    {
        width:min(500px, 95%);
        height:min(350px, 75vw);
        border-radius:10px;
        box-shadow:2px 2px grey;
        display: flex;
        flex-direction: column;
        background: white;
        padding:10px;
        
        
    }
    .project:hover
    {
        transform: scale(1.1);
        cursor:pointer
    }
    .project_title
    {
        text-align: center;
        
    }
    .project_description
    {
        color:blue;
        font-size: 20px;
    }
    .project_description::before
    {
        content:"\00a0 ";
    }
</style>