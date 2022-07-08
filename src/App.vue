<script setup>

</script>


<template>

  <main>
    <img src="./assets/logo.png" class="logo" />
    <div class="rowContent">
      <div class="columnOne">
        <button class="buttonColorFill"><svg width="16" height="17" viewBox="0 0 16 17" fill="none"
            xmlns="http://www.w3.org/2000/svg">
            <path
              d="M12 5.83334C12 4.77248 11.5786 3.75506 10.8284 3.00492C10.0783 2.25477 9.06087 1.83334 8 1.83334C6.93913 1.83334 5.92172 2.25477 5.17157 3.00492C4.42143 3.75506 4 4.77248 4 5.83334C4 10.5 2 11.8333 2 11.8333H14C14 11.8333 12 10.5 12 5.83334Z"
              stroke="white" stroke-width="1.33333" stroke-linecap="round" stroke-linejoin="round" />
            <path
              d="M9.15335 14.5C9.03614 14.7021 8.86791 14.8698 8.6655 14.9864C8.46309 15.1029 8.2336 15.1643 8.00001 15.1643C7.76643 15.1643 7.53694 15.1029 7.33453 14.9864C7.13212 14.8698 6.96389 14.7021 6.84668 14.5"
              stroke="white" stroke-width="1.33333" stroke-linecap="round" stroke-linejoin="round" />
          </svg>
          Avise-me</button>
        <button class="buttonOutlined">
          <a href="https://store.playstation.com/pt-br/pages/latest" target="_blank">
            Comprar
          </a>
        </button>
      </div>

      <div class="columnTwo">
        <h1 class="trailersTitle"> Trailers </h1>
        <div>
          <a href="https://www.youtube.com/watch?v=dIQGI36BxDE" target="_blank">
            <img src="./assets/video1.png" class="thumbVideo" />
          </a>

        </div>
        <div>
          <a href="https://www.youtube.com/watch?v=1McSEGBcQ70" target="_blank">
            <img src="./assets/video2.png" class="thumbVideo" />
          </a>

        </div>
      </div>


    </div>

    <div class="linksBottom">
      <ul>
        <li class="mr-25"><strong> Social </strong></li>

        <li><a href="https://www.linkedin.com/company/santa-monica-studio/" target="_blank"> Linkedin </a></li>
        <li><a href="https://www.youtube.com/c/PlayStation" target="_blank"> Youtube </a></li>
      </ul>
    </div>


  </main>

</template>

<style>
@import './assets/base.css';

ul {
  display: inline-flex;
  color: #fff;
  margin: 0;
  padding: 0;
  list-style: none;

}

a {
  text-decoration: none;
  color: #fff;
}

li,
li a {
  font-style: normal;
  font-size: 24px;
  line-height: 29px;
  text-transform: uppercase;
  color: #E7E7E7;
  text-decoration: none;
  margin-right: 1rem;
  transition: all ease 0.5s;

}

li:hover,
li a:hover {

  transform: scale(0.9);
}

main {
  font-family: 'Nunito', sans-serif;
  background-image: url('./assets/bg.jpg');
  width: 100%;
  height: 100vh;
  background-position: center;
  background-size: cover;
  background-position-y: inherit;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-around;

}

button {
  border: unset;
  cursor: pointer;
  margin-right: 1rem;
  border-radius: 4px;
  padding: 12px 32px;
  font-weight: 300;
  font-size: 18px;
  line-height: 25px;
  text-transform: uppercase;
}

.buttonColorFill {
  display: flex;
  justify-content: center;
  align-items: center;
  transition: all ease 0.5s;
  gap: 10px;
  background: #0080C8;
  color: #fff;
  border: 2px solid #0080C8;

}

.buttonColorFill:hover {
  border: 2px solid #FFFFFF;
  background: transparent;
  color: #fff;
}

.buttonOutlined {
  border: 2px solid #FFFFFF;
  border-radius: 4px;
  background: transparent;
  color: #fff;
  transition: all ease 0.5s;
}

.buttonOutlined:hover {
  background: #0080C8;
  border: 2px solid #0080C8;
}

.rowContent {
  display: flex;
  align-items: center;
  justify-content: space-around;
  gap: 250px;
}

.columnOne {
  display: flex;
  align-items: center;
  justify-content: center;
}

.trailersTitle {
  font-style: normal;
  font-weight: 600;
  font-size: 24px;
  line-height: 29px;
  text-transform: uppercase;
  color: #fff;
  margin-bottom: 1rem;
}

.logo {
  width: 500px;
  position: absolute;
  top: 0;
}

.thumbVideo {
  cursor: pointer;
  transition: all ease 0.5s;
  margin-bottom: 1rem;
}

.thumbVideo:hover {
  transform: scale(0.9);
}

.mr-25 {
  margin-right: 25rem;
}

.linksBottom {
  background: #2e6ba56e;
  width: 100%;
  position: absolute;
  bottom: 0;
  height: 163px;
  display: flex;
  align-items: center;
  justify-content: center;
}

@media (max-width: 993px) {
  .rowContent {
    display: block;
  }

  .trailersTitle {
    margin-top: 2rem;
  }

  ul,
  .columnOne,
  .linksBottom {
    display: block;
  }

  .logo {
    width: 270px;
  }

  ul {
    padding: 1rem;
  }

  .thumbVideo {
    width: 200px;
  }


}
</style>
