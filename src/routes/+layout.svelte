<script>
  import Header from "./Header.svelte";
  import Slogan from "./Slogan.svelte";
  import "./styles.css";
</script>

<div class="app">
  <div class="headerBg">
    <Header />

    <div class="slogan">
      <Slogan />
    </div>
  </div>

  <main>
    <slot />
  </main>

  <footer>
    <div class="footer">
      <div class="contain">
        <div class="col">
          <h1>Company</h1>
          <ul>
            <li>About</li>
            <li>Mission</li>
            <li>Services</li>
            <li>Social</li>
            <li>Get in touch</li>
          </ul>
        </div>
        <div class="col">
          <h1>Products</h1>
          <ul>
            <li>About</li>
            <li>Mission</li>
            <li>Services</li>
            <li>Social</li>
            <li>Get in touch</li>
          </ul>
        </div>
        <div class="col hidde">
          <h1>Accounts</h1>
          <ul>
            <li>About</li>
            <li>Mission</li>
            <li>Services</li>
            <li>Social</li>
            <li>Get in touch</li>
          </ul>
        </div>
        <div class="clearfix" />
      </div>
    </div>
  </footer>
</div>

<style>
  .app {
    display: flex;
    flex-direction: column;
  }

  .headerBg {
    background-color: #070617;
  }

  .slogan {
    margin: 0 30px 0 30px;
  }

  main {
    display: flex;
    flex-direction: column;
    align-items: center;
  }

  /* footer */
  .footer {
    margin-top: 20px;
    width: 100%;
    position: relative;
    height: auto;
    background-color: #070617;
  }

  .footer .col {
    width: 190px;
    height: auto;
    float: left;
    box-sizing: border-box;
    -webkit-box-sizing: border-box;
    -moz-box-sizing: border-box;
    padding: 0px 20px 20px 20px;
  }

  .footer .col h1 {
    margin: 0;
    padding: 0;
    font-family: inherit;
    font-size: 12px;
    line-height: 17px;
    padding: 20px 0px 5px 0px;
    color: rgba(255, 255, 255, 0.2);
    font-weight: normal;
    text-transform: uppercase;
    letter-spacing: 0.25em;
  }

  .footer .col ul {
    list-style-type: none;
    margin: 0;
    padding: 0;
  }

  .footer .col ul li {
    color: #999999;
    margin-left: 2px;
    font-size: 14px;
    font-family: inherit;
    font-weight: bold;
    padding: 5px 0px 5px 0px;
    cursor: pointer;
    transition: 0.2s;
    -webkit-transition: 0.2s;
    -moz-transition: 0.2s;
  }

  .social ul li {
    display: inline-block;
    padding-right: 5px !important;
  }

  .footer .col ul li:hover {
    color: #ffffff;
    transition: 0.1s;
    -webkit-transition: 0.1s;
    -moz-transition: 0.1s;
  }

  .clearfix {
    clear: both;
  }

  @media only screen and (min-width: 1280px) {
    .contain {
      width: 1200px;
      margin: 0 auto;
    }
  }

  @media only screen and (max-width: 950px) {
    .footer .col {
      width: 33%;
    }

    .footer .col h1 {
      font-size: 14px;
    }

    .footer .col ul li {
      font-size: 13px;
    }
  }

  @media only screen and (max-width: 500px) {
    .footer .col {
      width: 50%;
    }

    .footer .col h1 {
      font-size: 14px;
    }

    .footer .col ul li {
      font-size: 13px;
    }
	.hidde {
		display: none;
	}
  }

  @media only screen and (max-width: 340px) {
    .footer .col {
      width: 100%;
    }
  }
</style>
