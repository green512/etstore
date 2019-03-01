<template>
    <div>
        <iframe src="http://127.0.0.1:8000/docs/" width='100%' height='100%' frameborder='0' name="_blank" id="_blank" ></iframe>
    </div>
</template>
<script>
    var iframe = document.getElementById("_blank");
    var iwindow = iframe.contentWindow;
    var idoc = iwindow.document;
    iframe.height = idoc.body.offsetHeight;
</script>
<style  lang='scss'>
html {
    /*background:#fafafa;*/
    color:#333;
    _background-attachment:fixed
}

body,h1,h2,h3,h4,h5,h6,p,ul,ol,li,button,input {
    margin:0;
    padding:0;
    overflow: hidden;
}
body,button,input {
    font:12px/1.5 "Microsoft YaHei",Tahoma,Helvetica,Arial,simsun
}
em,i {
    font-style:normal
}
ul{
    list-style:none
}
img {
    border:0
}
h1 {
    font-size:18px
}
h2 {
    font-size:14px;
    font-weight:bold
}
h3 {
    font-size:14px;
    font-weight:400
}
h4,h5 {
    font-size:12px;
    font-weight:400
}
input,button {
    font-size:12px;
    outline:0;
    resize:none;
    color:#333
}
button {
    cursor:pointer
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

a:focus,area:focus {
    outline:0
}

canvas {
    -ms-touch-action:double-tap-zoom
}

.gray999,.gray,a.gray,a.gray:hover {
    color:#999
}

</style>
