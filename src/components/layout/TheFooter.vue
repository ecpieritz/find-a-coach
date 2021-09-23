<template>
  <footer>
    <h3>{{message}}</h3>

    <div class="socials">
      <a href="https://www.linkedin.com/in/ecpieritz/" target="_blank" rel="noopener noreferrer">
        <img id="linkedin" src="https://github.com/ecpieritz/png-logos/blob/main/linkedin-white.png?raw=true" alt="Linkedin">
      </a>

      <a href="https://www.instagram.com/ecpieritz/" target="_blank" rel="noopener noreferrer">
        <img id="instagram" src="https://github.com/ecpieritz/png-logos/blob/main/instagram-white.png?raw=true" alt="Instagram">
      </a>
      
      <a href="https://github.com/ecpieritz" target="_blank" rel="noopener noreferrer">
        <img id="github" src="https://github.com/ecpieritz/png-logos/blob/main/github-white.png?raw=true" alt="Github">
      </a>
    </div>
  </footer>
</template>

<script>
export default {
  data(){
    return{
      message: 'Developed with 💙 by Emilyn C. Pieritz'
    }
  }
};
</script>

<style scoped>
  footer{
    width: 100%;
    height: 4rem;
    background-color: #74146c;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
    position: fixed;
    bottom: 0;
    width: 100%;
  }

  footer h3{
    color: #fff;
    margin-left: 2rem;
  }

  footer .socials{
    margin: auto;
    display: flex;
    flex-direction: row;
    width: 110px;
    justify-content: space-between;
    margin-right: 2rem;
  }

  footer .socials #linkedin, .socials #instagram, .socials #github{
  width: 30px;
}
</style>