<button on:click={openAstray}>
     <img src="assets/games/astray.png" alt="Astray Pic" width="225" height="225">
</button>

<script>
function openAstray() {
  window.open('https://doordashv2.devendyer.repl.co/games/astray/index.html');
}
</script>


<style>
  button {
    cursor:pointer;
    background-color:#404757;
    border:4px solid black;
    border-radius:10px;
  }

  button:hover {
    border-radius:10px;
  }
</style>