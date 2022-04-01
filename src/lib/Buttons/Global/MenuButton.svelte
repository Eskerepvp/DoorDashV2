<button on:click={loadMenu}>
     <img src="assets/global/menuBars.png" alt="Menu Bars" width="12" height="12"> 
</button>

<script>
    function loadMenu() {
       var x = document.getElementById("items");
  if (x.style.display === "none") {
    x.style.display = "block";
  } else {
    x.style.display = "none";
  }
    }
</script>


<style>
  button {
    padding:8px;
    position:fixed;
    top:0;
    right:0;
    border:none;
    background-color:#161923;
  }

  button:hover {
    position:fixed;
    background-color:#3A3B3C;
  }
</style>