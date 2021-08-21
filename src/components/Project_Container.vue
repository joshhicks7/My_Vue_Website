<template>
    <div class="project_container">
        <div class = "pc_header"><h2> MY PROJECTS </h2></div>        
        <Project  title="MY WEBSITE" description="This website was made by me. It took work to do it but I did it"/>
        <Project  title="JavaScript" description="I can write all the web applications in Javascript that your heart will ever desire"/>
        <Project  title="HTML" description="I provide very well HTML sites. They are quite responsive"/>
        <Project  title="Champion Pie Eater" description="I was awarded this medal after eating 17 pies in 5 minutes. (This is not true)"/>
        <Project  title="Facebook Clone" description=" Facebook clone web application using React. It include Google authentication." link = "http://joshhicks7.github.io/facebook-clone"/>
        <Project title = "Tic Tac Toe" description="This is a tic tac toe game created in Angular." link = "http://joshhicks7.github.io/angular-tic-tac-toe"/>
    </div>
</template>

<script>
import Project from './Project.vue'

export default 
{
  components: { Project },
    name:'Project_Container'    
}
</script>

<style scoped>
    .project_container
    {
       /* background: black;*/     
        display:flex;
        flex-wrap: wrap;
        row-gap:25px;
        column-gap: 25px;
        padding:10px;
        padding-top:100px;
        justify-content:space-evenly;
    }
    
    .pc_header
    {
        color:white;
        flex-basis: 100%;
        text-align: center;
    }
</style>
