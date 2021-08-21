<template>
    <div class = "aboutme">
        <div class="aboutme_left">
            
        </div>
        <div class="aboutme_middle">

        </div>
        <div class="aboutme_right">
            <h2 style = "text-decoration:underline">ABOUT ME</h2>
            <p class = "text">
                Let this be a test project for the Arkansas coding Academy. It went pretty well. Vue is actually kind of fun. There are some thing I like better in it than in react, but there are also some things that are better in React than this. 
            </p>
        </div>
    </div>
</template>

<script>


export default 
{
    name:"AboutMe"
}

</script>

<style scoped>
    .aboutme
    {
        display: flex;
        flex-wrap: wrap;
        color:white;
        gap:10px;
        justify-content: space-evenly;
        padding:10px;
        padding-top:100px;
    }
    .text
    {
        overflow: wrap;
        width:min(500px,100vw - 20px);
        padding:10px;
    }
    .aboutme_right
    {
        text-align: center;
    }
    .aboutme_left
    {
        background: url("https://joshhicks7.github.io/Files/images/me.png");
        background-repeat: no-repeat;
        background-size:cover;
        width:350px;
        height:350px;
    }
</style>
