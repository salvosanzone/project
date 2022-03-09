<template>

  <header>
    <div class="menu d-flex align-items-baseline">
      <div class="container-fluid">
        <div class="row align-items-baseline">
          <div class="col-4">
            <div class="menu-left">
              <ul>
                <li>
                  <a href="#">prodotti</a>
                </li>
                <li>
                  <a href="#">collezioni</a>
                </li>
                <li>
                  <a href="#">progetti</a>
                </li>
                <li>
                  <a href="#">inspiration</a>
                </li>
                <li>
                  <a href="#">designer</a>
                </li>
              </ul>
            </div>
          </div>
          <div class="col-4 d-flex justify-content-center">
            <div class="menu-center">
              <a href="#">
                <img class="logo" src="../assets/style/icons/logo.svg" alt="">
              </a>
              
            </div>
          </div>
          <div class="col-4">
            <div class="menu-right">
              <ul>
                <li>
                  <a href="#">About</a>
                </li>
                <li>
                  <a href="#">Stories</a>
                </li>
                <li>
                  <a href="#">Cataloghi</a>
                </li>
                <li>
                  <a href="#">Showroom</a>
                </li>
                <li>
                  <a href="#">
                    <img src="../assets/style/icons/search.svg" alt="">
                  </a>
                </li>
                <li>
                  <a href="#">
                    <img src="../assets/style/icons/user.svg" alt="">
                  </a>
                </li>
                <li>
                  <a href="#">
                    <img src="../assets/style/icons/cart.svg" alt="">
                  </a>
                </li>
              </ul>
            </div>
            
          </div>
        </div>
      </div>
    </div>
    <img class="background" src="../assets/img/desktop/00_hero.jpg" alt="00_hero">
    <div class="overlay"></div>
    <div class="text">
      
      <div class="top-text">Lorem ipsum sit</div>
      <div class="center-text">Eiusdem loci, <br> sit dolor amet neque</div>
      <div class="bottom-text">
        <di class="btn btn-outline-light">Scopri la collezione</di>
      </div>
    </div>
  </header>
  

</template>

<script>
export default {
    name: 'MyHeader',
    data() {
      return {
        isActive: false
      }
    }
}
</script>

<style lang="scss" scoped>
header {
  position: relative;
  display: flex;
  justify-content: center;
  align-items: center;
  width: 100%;
  height: 100vh;

  .background {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    object-fit: cover;
    object-position: center;
  }

  .text {
    z-index: 1;
    text-align: center;
    color: white;

    .top-text {
      font-size: 18px;
    }

    .center-text {
      font-size: 80px;
      line-height: 80px;
    }

  }
  .overlay {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: rgba($color: #000000, $alpha: 0.5);
  }

  .menu {
    position: absolute;
    top: 0;
    left: 0;
    z-index: 1;
    width: 100%;
    height: 84px;
    padding: 20px;

    .menu-left {
      text-transform: uppercase;
      display: flex;
      justify-content: center;

      ul {
        display: flex;

        li {
          list-style: none;
          margin: 0 5px;

          a {
            text-decoration: none;
            height: 19px;
            width: 97px;
            color: black;
            font-family: Quicksand;
            font-size: 15px;
            font-weight: 500;
            letter-spacing: 0.5px;
            line-height: 19px;

            &:hover {
              color: #474E4B;
            }
          }
        }
      }
    }

    .box {
      height: 100%;
    }

    .menu-center {
      
      .logo {
        width: 146px;
        height: 24px;
      }
    }
    .menu-right {
      text-transform: none;

      ul {
        display: flex;
        
        li {
          list-style: none;
          margin: 0 5px;

          a {
            text-decoration: none;
            height: 19px;
            width: 44px;
            color: black;
            font-family: Quicksand;
            font-size: 15px;
            letter-spacing: 0.5px;
            line-height: 19px;

            &:hover {
             color: #474E4B;
            }
          }
        }
      }

    }
  }
}

</style>