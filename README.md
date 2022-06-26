<img src="https://raw.githubusercontent.com/arturssmirnovs/arturssmirnovs/master/banner.png" alt="Banner about Arturs Smirnovs">

<h1> Howdy!, I am <a href="https://github.com/Defcon27">Tiandong Li</a> <h1> <img src="https://raw.githubusercontent.com/ABSphreak/ABSphreak/master/gifs/Hi.gif" height="30px"> </h1>

### A little about me...  <img src="https://media.giphy.com/media/VgCDAzcKvsR6OM0uWg/giphy.gif" width="50"> 
I'm an **Undergrad Student🎓 [@VIT Vellore](https://www.vit.ac.in)** pursuing CSE. I'm a **Tech Enthusiast 💻 😃** passionate about learning and working with new tech. I love building interesting and amazing products that serve a great deal of purpose. <br/><br/>

#### TECH STACK

PHP / MYSQL / SOLR / FLUTTER / DART / JS / NODE JS / JQUERY / HTML / CSS / SCSS / LESS / BOOSTRAP / LARAVEL / YII2 / CODIGNITER / UNIX / GITHUB / SVN / APACHE / NGINX / REST API / NATIVE SCRIPT / AZURE / GOOGLE API's

##### MOTTO

> 语雀：**[左手柳叶刀右手炭火烧](#jump_10)**
> 微信公众号：**[研平方](#jump_10)**  |  简书：**[研平方](#jump_10)** 


####

<a href="https://www.facebook.com/artuurs.smirnovs" target="_blank"><img src="https://raw.githubusercontent.com/arturssmirnovs/arturssmirnovs/master/fb.png" alt="Facebook" width="30"></a>
<a href="https://twitter.com/artuurssmirnovs" target="_blank"><img src="https://raw.githubusercontent.com/arturssmirnovs/arturssmirnovs/master/tw.png" alt="Twitter" width="30"></a>
<a href="https://www.instagram.com/arturssmirnovs/" target="_blank"><img src="https://raw.githubusercontent.com/arturssmirnovs/arturssmirnovs/master/ig.png" alt="Instagram" width="30"></a>
<a href="https://www.linkedin.com/in/art%C5%ABrs-smirnovs-b6399275/" target="_blank"><img src="https://raw.githubusercontent.com/arturssmirnovs/arturssmirnovs/master/in.png" alt="LinkedIn" width="30"></a>
<a href="https://github.com/arturssmirnovs" target="_blank"><img src="https://raw.githubusercontent.com/arturssmirnovs/arturssmirnovs/master/git.png" alt="GitHub" width="30"></a>
<a href="https://arturio.dev/" target="_blank"><img src="https://raw.githubusercontent.com/arturssmirnovs/arturssmirnovs/master/www.png" alt="Website" width="30"></a>

![Profile views](https://gpvc.arturio.dev/arturssmirnovs?v=3)


<div id="header" align="center">
  <img src="https://media.giphy.com/media/M9gbBd9nbDrOTu1Mqx/giphy.gif" width="100"/>
</div>

<h1>
  hey there
  <img src="https://media.giphy.com/media/hvRJCLFzcasrR4ia7z/giphy.gif" width="30px"/>
</h1>

> 语雀：**[左手柳叶刀右手炭火烧](#jump_10)**

微信公众号：**[研平方](#jump_10)**  |  简书：**[研平方](#jump_10)** 

关注可了解更多的科研教程及技巧。如有问题或建议，请留言。

**[欢迎关注我：一起学习，一起进步！](#jump_20)**


name: Latest blog post workflow
on:
  schedule: # Run workflow automatically
    - cron: '0 * * * *' # Runs every hour, on the hour
  workflow_dispatch: # Run workflow manually (without waiting for the cron to be called), through the Github Actions Workflow page directly

jobs:
  update-readme-with-blog:
    name: Update this repo's README with latest blog posts
    runs-on: ubuntu-latest
    steps:
      - name: Checkout
        uses: actions/checkout@v2
      - name: Pull in dev.to posts
        uses: gautamkrishnar/blog-post-workflow@v1
        with:
          feed_list: "https://dev.to/feed/gautamkrishnar,https://www.gautamkrishnar.com/feed/"
