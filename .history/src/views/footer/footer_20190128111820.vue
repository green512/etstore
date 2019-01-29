<template>
<div id="footer">
    <div class="ft-bg">
        <div class="w-ensure mb20">
            <div class="w-main">
                <ul>
                    <li>精度为90-96%</li>
                    <li>世行项目支持</li>
                    <li>定制ET遥感</li>
                    <li>节水效果评估</li>
                </ul>
            </div>

        <div class="ft_main">
            </div>
            <div class="ft_txt">
                <p class="ft_contact"> <span>服务时间：09:00-18:00</span>
                    <span class="ft_phone">客服热线: <em>010-88888888</em></span>
                </p>
            </div>
            <div class="ft_txt">
          <div class="container">
              <div class="footer-wrap idx-width">
                    <div class="footer-sns clearfix">
                         <div class="l">
                         </div>
                         <div class="l">  </div> 
                         </div>    </div> 
                           <div class="footer-link">   
                                <!-- <a href="/about/us" target="_blank" title="关于我们">关于我们</a> -->  
                                      <a href="/about/job" target="_blank" title="人才招聘">人才招聘</a> 
                                        <a href="/about/contact" target="_blank" title="联系我们">联系我们</a> 
                                        <a href="/help" target="_blank" title="帮助中心">帮助中心</a>
                                        <a href="/user/feedback" target="_blank" title="意见反馈">意见反馈</a>
                                        <a href="/about/friendly" target="_blank" title="友情链接">友情链接</a>    </div>  
                             <div class="footer-copyright">     <p>©&nbsp2019&nbspetwatch.cn&nbsp&nbsp京ICP备 12003892号-11</p>    </div> 
                             </div></div>

    </div>
        </div>
        
</div>
</template>
<script>

</script>
<style scoped  lang='scss'>

html {
    background:#fafafa;
    color:#333;
    _background-attachment:fixed
}
html.isPhone {
    min-width:1196px
}
body,p {
    margin:0;
    padding:0
}
body{
    font:12px/1.5 "Microsoft YaHei",Tahoma,Helvetica,Arial,simsun
}
i {
    font-style:normal
}
ul {
    list-style:none;
    height: 90px;
}

img {
    border:0
}
a {
    text-decoration:none;
    color:#333;
    -webkit-transition:color .2s;
    -moz-transition:color .2s;
    -o-transition:color .2s;
    -ms-transition:color .2s;
    transition:color .2s
}
a:hover {
    color:#0e90d2
}
a:focus,area:focus {
    outline:0
}



#footer {
    border-top:1px solid #eee;
    background:#fff;
}
#footer .ft_main {
    width:1196px;
    margin:0 auto
}
#footer .ft_cata {
    display:none
}
#footer .w-ensure {
    background: #0e90d2 none repeat scroll 0 0;
    height: 90px;
}
#footer .w-main {
    margin: 0 auto;
    width: 1196px;
    height: 90px;
}
#footer ul{
    margin: auto;
}
#footer .w-main::after {
    clear: both;
    content: "";
    display: table;
}
#footer .w-ensure li {
    float: left; 
    width:25%;
    height: 100%;
    color:#fff;
    font-size: 24px;
    font-weight:bold;
    text-align:center;
    /* Firefox */
    display:-moz-box;
    -moz-box-pack:center;
    -moz-box-align:center;

    /* Safari, Chrome, and Opera */
    display:-webkit-box;
    -webkit-box-pack:center;
    -webkit-box-align:center;

    /* W3C */
    display:box;
    box-pack:center;
    box-align:center

}
#footer .ft_nav {
    height:22px;
    padding:20px 0 15px;
    text-align:center
}
#footer .ft_nav a {
    display:inline-block;
    padding:0 20px 0 20px;
    /*background:url(../../../static/images/footer/border-right.png) no-repeat 0 center*/
}
#footer .ft_nav a.noborder {
    background:0
}

#footer .ft_txt {
    text-align:center;
    padding:8px 0;
    font-size:14px
}
#footer .ft_txt p {
    padding:5px 0;
    color:#666
}

#footer .ft_txt .ft_phone em {
    color:#0e90d2;
    font-size:18px
}
#footer .ft_txt .ft_contact span {
    display:inline-block;
    padding:0 10px
}

#footer .footer-link a{
    margin:10px;
    font-size:14px
}

</style>
