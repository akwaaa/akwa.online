<script>
  import { Router, Link, Route } from "svelte-routing";
  import Home from "./routes/Home.svelte";
  import About from "./routes/About.svelte";
  import Contact from "./routes/Contact.svelte";
  import Setup from "./routes/Setup.svelte";
  import Portfolio from "./routes/Portfolio.svelte";
  import Title from "./lib/title.svelte";

  export let url = "";
</script>

<Router {url}>
  <Title/>
<h1 class="navbar">
  <a href="/">home</a> -
  <a href="/about">about me</a> -
  <a href="/contact">contact</a> -
  <a href="/setup">setup</a> -
  <a href="/portfolio">portfolio (soon)</a>
</h1>
<hr>
<!-- svelte-ignore a11y-distracting-elements -->
<marquee class="scroll" scrolldelay="10" truespeed scrollamount="3">now playing: [soon™] - discord status: [soon™]</marquee>
<hr>
  <div>
    <Route path="/portfolio" component={Portfolio} />
    <Route path="/setup" component={Setup} />
    <Route path="/contact" component={Contact} />
    <Route path="/about" component={About} />
    <Route path="/"><Home /></Route>
  </div>
</Router>

<style>

  h1.navbar {
      color: white;
      text-align: center;
      font-size: 36px;
      font-family: Inter;
      font-weight: 400;
      word-wrap: break-word 
  }
  
  marquee.scroll {
      color: white;
      font-size: 24px;
      font-family: Inter;
      font-weight: 400;
      word-wrap: break-word;
      line-height: 1.2;
  }
  
  hr {
      color: white;
  }
  
  a:link {
      color: #cbeaff;
      background-color: transparent;
      text-decoration: none;
  }
  
  a:visited {
      color: #cbeaff;
      background-color: transparent;
      text-decoration: none;
  }
  
  a:hover {
      color: rgb(255, 255, 255);
      background-color: transparent;
      text-decoration: underline;
  }
  
  a:active {
      color: #7acaff;
      background-color: transparent;
      text-decoration: underline;
  }
  
  
  </style>