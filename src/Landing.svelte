<script>
  import { link } from "svelte-routing";
	import Navbar from "./Navbar.svelte";
  import Footer from './Footer.svelte';
  import Section from './Section.svelte';
  import logo from '../public/img/SvelteStorm4Logo10x1024.png'
</script>

<Navbar />
<main>
  <div class="relative pt-28 pb-48 flex content-center items-center justify-center min-h-screen-75">
    <div
    class="absolute top-0 w-full h-full bg-center bg-cover bg-indigo-900"
    >
    <center>
      <img src={logo} alt='SvelteStorm Logo' id='logo' width=600 height=600>
    </center>
    </div>
    <div class="container relative mx-auto">
      <div class="items-center flex flex-wrap">
        <div class="w-full lg:w-6/12 px-4 ml-auto mr-auto text-center">
          <div class="headerText">
            <h1 class="text-white font-semibold text-5xl">
              Welcome to SvelteStorm
            </h1>
            <div class="mt-4 text-lg text-white">
              <h2>A Svelte IDE</h2>
              <h3>Embrace the Storm.</h3>
            </div>          
          </div>
        </div>
      </div>
    </div>
    <div
      class="top-auto bottom-0 left-0 right-0 w-full absolute pointer-events-none overflow-hidden h-70-px"
      style="transform: translateZ(0);"
    >
      <svg
        class="absolute bottom-0 overflow-hidden"
        xmlns="http://www.w3.org/2000/svg"
        preserveAspectRatio="none"
        version="1.1"
        viewBox="0 0 2560 100"
        x="0"
        y="0"
      >
        <polygon
          class="text-blueGray-200 fill-current"
          points="2560 0 2560 100 0 100"
        ></polygon>
      </svg>
    </div>
  </div>


  

  <section class="pb-20 bg-gray-100 -mt-24">
    <div class="container mx-auto px-4">
      <div class="flex flex-wrap">
        <div class="lg:pt-12 pt-6 w-full md:w-4/12 px-4 text-center">
          <div
            class="relative flex flex-col min-w-0 break-words bg-white w-full mb-8 shadow-lg rounded-lg"
          >
            <div class="px-4 py-5 flex-auto">
              <div
                class="text-white p-3 text-center inline-flex items-center justify-center w-12 h-12 mb-5 shadow-lg rounded-full bg-red-400"
              >
                <i class="fa-brands fa-chrome"></i>
              </div>
              <h6 class="text-xl font-semibold">Browser Window</h6>
              <p class="mt-2 mb-4 text-blueGray-500">
                SvelteStorm's built-in browser window allows for developers to easily view their application 
                without having to switch to a separate window! 
                This feature increases efficiency and creates a smooth coding experience.
              </p>
            </div>
          </div>
        </div>

        <div class="w-full md:w-4/12 px-4 text-center">
          <div
            class="relative flex flex-col min-w-0 break-words bg-white w-full mb-8 shadow-lg rounded-lg"
          >
            <div class="px-4 py-5 flex-auto">
              <div
                class="text-white p-3 text-center inline-flex items-center justify-center w-12 h-12 mb-5 shadow-lg rounded-full bg-blue-400"
              >
                <i class="fa-solid fa-clock-rotate-left"></i>
              </div>
              <h6 class="text-xl font-semibold">Time Travel Debugger</h6>
              <p class="mt-2 mb-4 text-blueGray-500">
                SvelteStorm's Time Travel Debugging tool allows developers to capture snapshots of a running application and 
                change the current state in real-time, making it easier than ever to chase down bugs. 
              </p>
            </div>
          </div>
        </div>

        <div class="pt-6 w-full md:w-4/12 px-4 text-center">
          <div
            class="relative flex flex-col min-w-0 break-words bg-white w-full mb-8 shadow-lg rounded-lg"
          >
            <div class="px-4 py-5 flex-auto">
              <div
                class="text-white p-3 text-center inline-flex items-center justify-center w-12 h-12 mb-5 shadow-lg rounded-full bg-green-400"
              >
                <i class="fa-solid fa-cloud-arrow-down"></i>
              </div>
              <h6 class="text-xl font-semibold">Quick and Easy Download</h6>
              <p class="mt-2 mb-4 text-blueGray-500">
                SvelteStorm distributables are in progress so keep your eyes out! For now, 
                developers can easily clone down our repo and hop right into the this fresh Svelte coding experience. 
                Follow the instructions below to try out SvelteStorm!
              </p>
            </div>
          </div>
        </div>
      </div>


      <div class="flex flex-wrap items-center mt-32">
        <div class="w-full md:w-5/12 px-4 mr-auto ml-auto">
          <div
            class="text-blueGray-500 p-3 text-center inline-flex items-center justify-center w-16 h-16 mb-6 shadow-lg rounded-full bg-white"
          >
            <i class="fa-solid fa-download text-xl"></i>
          </div>
          <h3 class="text-3xl mb-2 font-semibold leading-normal">
            How to Download
          </h3>
          <p
            class="text-lg font-light leading-relaxed mt-4 mb-4 text-blueGray-600"
          >
          SvelteStorm is unbelievably easy to use and install! 
          Distributables are in progress for Mac (M1 Chip specific), Linux, and Windows machines.
          </p>
          <p
            class="text-lg font-light leading-relaxed mt-0 mb-4 text-blueGray-600"
          >
          For the time being, head over to our main repo on <a href="https://github.com/open-source-labs/SvelteStorm" target="_blank"><b>GitHub</b></a>. 
          All you have to do is fork, clone and npm install our lovely IDE.
          </p>
          <p>
            Happy Coding!
          </p>
        </div>

        <div class="w-full md:w-6/12 px-4 mr-auto ml-auto">
          <div
            class="relative flex flex-col min-w-0 break-words bg-white w-full mb-6 shadow-lg rounded-lg bg-red-400"
          >
            <img
              alt="..."
              src="https://s4.gifyu.com/images/ezgif.com-gif-maker9a35bac3e8702a7d.gif"
              class="max-w-full rounded-lg shadow-lg"
            />
          </div>
        </div>
      </div>
    </div>
  </section>

  <Section />

  <Footer />
</main>

<style global lang="postcss">
  @tailwind base;
  @tailwind components;
  @tailwind utilities;

  /* #landing-container{
    content: ' ';
    display: block;
    position: absolute;
    left: 0;
    top: 0;
    width: 100%;
    height: 100%;
    opacity: 0.3;
    background-image: url('SvelteStorm4Logo10x512.png');
    box-shadow: 15px 15px 50px 0 rgb(0, 0, 0) inset, -15px -15px 50px 0 rgb(0, 0, 0) inset;
    background-repeat: no-repeat;
    background-position: 50% 0;
    background-size: cover;
  }
   */
  #logo {
    -webkit-filter: blur(2px);
    position: relative;
    top: -100px;
    filter: brightness(75%)
  }
  .headerText{
    text-shadow: 2px 2px 4px #000000
  }
  
</style>

