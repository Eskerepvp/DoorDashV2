<button on:click={openTetris}>
     <img src="assets/games/tetris.webp" alt="Tetris Pic" width="225" height="225">
</button>

<script>
function openTetris() {
  window.open('https://doordashv2.devendyer.repl.co/games/tetris/index.html');
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