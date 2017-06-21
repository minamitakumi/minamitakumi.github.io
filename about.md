---
layout: default
title: About - 
---

<!-- Language Selector -->
<select style="background-color: #202020; color: #fbfbfb;" onchange= "onLanChange(this.options[this.options.selectedIndex].value)">
    <option value="0" selected> 中文 </option>
    <option value="1"> English </option>
</select>

<!-- Chinese Version -->
<div class="zh">
    <p>你好，我是<strong>wassery</strong>，目前投身于游戏行业。我喜欢游戏编程技术！</p>

    <p>爱好写代码。</p>

    <p>联系方式：wassery_zhou # 163 DOT com</p>
</div>

<!-- English Version -->
<div class="en">
    <p>Hi, my name is <strong>wassery</strong>. Currently I am working in game industry and code for it!</p>

    <p>I like coding.</p>

    <p>Contact me：wassery_zhou # 163 DOT com</p>
</div>

<!-- Handle Language Change -->
<script type="text/javascript">
    var $zh = document.querySelector(".zh");
    var $en = document.querySelector(".en");
    function onLanChange(index){
        if(index == 0){
            $zh.style.display = "block";
            $en.style.display = "none";
        }else{
            $en.style.display = "block";
            $zh.style.display = "none";
        }
    }
    onLanChange(0);
</script>