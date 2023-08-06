<script>
  import Title from "./lib/title.svelte";
  import Word from "./lib/word.svelte";
</script>

<main>
<Title/>
<h1 class="navbar"><a href="https://akwa.online/">home</a> - portfolio - contact - setup - bonus</h1>
<hr>
<!-- svelte-ignore a11y-distracting-elements -->
<marquee class="scroll" scrolldelay="10" truespeed scrollamount="3">now playing: [soon™] - discord status: [soon™]</marquee>
<hr>
<br>
<div class="container">
  <div>
    <img class="pfp" src="src/assets/pfp.png" width="230px" alt="profile pic">
  </div>
  <div>
    <Word/>
    <h1>freeparty enjoyer, amateur dj | free tekno for free people &lt;3</h1>
    <h1>
      <a href="https://soundcloud.com/eatincatfood">soundcloud</a> - 
      <a href="https://open.spotify.com/user/isyg8ky5hrcmptz626tcn35n5?si=4e4fc2c03e8b49fc">spotify</a> - 
      <a href="https://github.com/Akwaaa">github</a> - 
      <a href="https://twitch.tv/444Akwa">twitch</a> - 
      <a href="https://instagram.com/eatincatfood">insta</a> - 
      <a href="https://last.fm/user/akwajpn">last.fm</a> - 
      <a href="https://steamcommunity.com/id/616b7761">steam</a>
    </h1>
    <h1>
      <a href="https://blahaj.systems">blåhaj</a> x 
      <a href="https://steamcommunity.com/groups/thetacrewcsgo">theta</a> x 
      <span class="nolink">bdv</span> x 
      <span class="nolink">dea</span>
    </h1>
  </div>
</div>
</main>

<style>
  :root {
    background: #C082FF;
    margin-left: 15%;
    margin-right: 15%;
  }

  h1.navbar {
    color: white;
    text-align: center;
    font-size: 36px;
    font-family: Inter;
    font-weight: 400;
    word-wrap: break-word 
  }

  h1 {
    color: white;
    font-size: 30px;
    font-family: Inter;
    font-weight: 400;
    word-wrap: break-word;
    line-height: 1;
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

  .container {
    display: flex;
    flex-direction: row;
  }

  img.pfp {
    margin-left: 40px;
    margin-right: 30px;
    border-radius: 10%;
  }

  .nolink {
    color: #cbeaff;
  }
</style>