<template>
    <div class = "header">
        <div class="header_top">
            <h1>
                This is Me (Josh)
            </h1>
        </div>
        <div class="header_bottom">
           <div class = "scrollTop" @click="scroll('aboutme')">About Me</div>
            <div class = "scrollTop" @click ="scroll('project_container')">My Projects</div>
            <div class = "scrollTop" @click ="scroll('contact')">Contact Me</div>
        </div>
    </div>
</template>

<script>
export default 
{
  name: 'Header',
  methods:
  {
      scroll(clas)
      {
          document.getElementsByClassName(clas)[0].scrollIntoView({behavior:"smooth"})
      }
  }
}
</script>
   
<style scoped>
 .header
    {       
        background: white;
        box-shadow:1px 1px 1px 1px grey;
        display: flex;
        flex-direction: column;
        justify-content: space-evenly;
        z-index: 500;
        position: sticky;
        top:0px;
        text-align: center;
    }

    h1
    {
        text-transform: uppercase;
    }
    
    .header_bottom
    {
        display: flex;
        flex-direction: row;
        justify-content:space-evenly;
    }
    .scrollTop
    {
        text-decoration: underline;
        font-size:20px;

    }
    .scrollTop:hover
    {
        cursor:pointer;
        color:blue;
    }
</style>
