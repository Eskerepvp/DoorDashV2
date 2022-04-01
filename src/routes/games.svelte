<script>
  import MenuButton from '$lib/Buttons/Global/MenuButton.svelte'
  import TetrisButton from '$lib/Buttons/Games/TetrisButton.svelte'
  import Ohh1Button from '$lib/Buttons/Games/Ohh1Button.svelte'
  import AstrayButton from '$lib/Buttons/Games/AstrayButton.svelte'
</script>

<style>

  :root {
   background-color:#161923;
   font-family:monospace;
  }

  main {
    text-align: center;
    padding: 1em;
    margin: 0 auto;
  }
  
  .menuStip {
      border-radius:10px;
      color:white;
      display:inline-block;
      font-size:18px;
      font-family:inherit;
      width:95%;
      padding: 15px; 
      text-align:center;
      background-color:#404757;
      border:2px solid #404757;
  }

  .home {

  position:relative;
    
  color: inherit;

  margin-right:50px;
 
  text-decoration: none;
  }


  .proxies {

  position:relative;
    
  color: inherit;

  margin-right:50px;
 
  text-decoration: none;
  }
  .games {

  position:relative;

  margin-right:50px;
    
  color: inherit; 
    
  text-decoration: none;
  }
  .apps {

  margin-right:50px;
    
  position:relative;
    
  color: inherit; 
    
  text-decoration: none;
  }

  .dropDownMenu {
  position: fixed;
  top:0;
  right:0;
  border:none;
  border-radius:5px;
  color:white;
  display:inline-block;
  font-size:13px;
  font-family:inherit;
  background-color:#161923;
  border:2px solid #404757;
  }

  .settings {
  text-decoration: none;
  color: inherit;
  }

  .credits {
  text-decoration: none;
  color: inherit;
  }

  .source {
  text-decoration: none;
  color: inherit;
  }

  ul {
    list-style-type: none;
}

  #items {
    list-style-type: none;
    display:none
  }


    h1 {
    color: white;
    font-size: 40px;
    font-weight: 100;
    line-height: 1.1;
    margin: 2rem auto;
    max-width: 14rem;
  }

  #tetrisDiv {
  border:none;
  border-radius:10px;
  color:white;
  display:inline-block;
  font-size:24px;
  font-family:inherit;
  position:relative; 
  background-color:#404757;
  border:10px solid #404757;
  }

  #tetrisDiv:hover {
  transform:scale(1.05);
  z-index:2;
  }

  #Ohh1Div {
  border:none;
  border-radius:10px;
  color:white;
  display:inline-block;
  font-size:24px;
  font-family:inherit;
  position:relative; 
  background-color:#404757;
  border:10px solid #404757;
  }

  #Ohh1Div:hover {
  transform:scale(1.05);
  z-index:2;
  }

  #AstrayDiv {
  border:none;
  border-radius:10px;
  color:white;
  display:inline-block;
  font-size:24px;
  font-family:inherit;
  position:relative; 
  background-color:#404757;
  border:10px solid #404757;
  }

  #AstrayDiv:hover {
  transform:scale(1.05);
  z-index:2;
  }

  @media (min-width: 480px) {
    h1 {
      max-width: none;
    }

    p {
      max-width: none;
    }
  }
  
</style>


<main>

  <div class="menuStip" id="menuStipId">

  <a href="/" class="home">Home</a>  
    
  <a href="/" class="proxies">Pr*xies</a>  
  <!-- TODO code proxie page -->
  <a href="/games" class="games" id="games">Games</a>
    <!-- TODO code games page -->
  <a href="/" class="apps">Apps</a>
    <!-- TODO code apps page -->
  </div>

  <div class ="dropDownMenu" id="menu"> 
    
  <MenuButton class="menuButton" id="MenuButtonId"/>
    
  <ul class = "items" id = "items">
  <li><a href="/about" class="settings">Settings</a></li>
  <li><a href="/" class="credits">Credits</a></li>
  <li><a href="/" class="source">Source</a></li> </ul>
  </div>

  <h1>
  Games
  </h1>

  
  <div id ="tetrisDiv">
  <TetrisButton/>
    <p id="tetrisText">
      Tetris
    </p>
  </div>
  
  <div id="Ohh1Div">
  <Ohh1Button/>
  <p id="Ohh1Text">
    0h h1
  </p>
  </div>

  <div id="AstrayDiv">
  <AstrayButton/>
  <p id="AstrayText">
    Astray
  </p>
  </div>
  
</main>
