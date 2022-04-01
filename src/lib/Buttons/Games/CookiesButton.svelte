<button on:click={openCookies}>
     <img src="assets/games/cookie.webp" alt="Cookies Pic" width="225" height="225">
</button>

<script>
function openCookies() {
  window.open('https://doordashv2.devendyer.repl.co/games/cookies/index.html');
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