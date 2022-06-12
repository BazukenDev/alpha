<script>
  import Button from "./components/button.svelte";
</script>

<header>
  <a class="logo" href="/">
    <img src="./img/a-logo-min.jpg" alt="Alpha Griechisches Restaurant" />
  </a>
  <div class="adress">
    <img src="./img/pin.png" alt="adress" class="pin" />
    <span class="text">Quellengasse 1, 96275 Marktzeuln</span>
    <img src="./img/down.png" alt="" class="down" />
  </div>
  <div class="info">
    <Button className="primary">
      <img src="./img/love.svg" alt="Favorite" class="love" />
    </Button>
  </div>
</header>

<style lang="scss">
  header {
    display: flex;
    justify-content: space-between;
    min-height: 60px;
    margin: 20px auto 0 auto;
    padding: 10px 0;
    max-width: 780px;

    .logo {
      width: 60px;
      height: 60px;
      flex: 0 0 auto;
      overflow: hidden;
      border-radius: 50%;

      img {
        width: 100%;
        height: 100%;
        object-fit: cover;
        object-position: center;
      }
    }

    .adress {
      display: flex;
      flex-flow: row nowrap;
      justify-content: center;
      align-items: center;
      flex: 1;
      font-size: 16px;
      line-height: 20px;
      font-weight: 600;
      text-align: center;
      padding: 5px 10px;

      .text {
        margin: 0 8px;
      }

      img {
        width: 20px;
        height: 20px;
        display: flex;
      }
    }

    .info {
      display: flex;
      width: 60px;
      height: 60px;
      flex: 0 0 auto;

      .button {
        margin: auto;
      }
    }
  }
</style>
