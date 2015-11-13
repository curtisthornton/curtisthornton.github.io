<!doctype html>
<html lang="en">
<head>
<meta charset="utf-8">
<title>{Title}{block:PostSummary} – {PostSummary}{/block:PostSummary}</title>
{block:Description}
<meta name="description" content="{MetaDescription}">
{/block:Description}
<meta name="author" content="Forward is a Tumblr theme by Andrew Revitt - http://andrewrevitt.com/themes/">
<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
<link rel="shortcut icon" href="{Favicon}">
<link rel="apple-touch-icon-precomposed" href="{PortraitURL-128}">
<link rel="alternate" type="application/rss+xml" href="{RSS}">
<link href="http://fonts.googleapis.com/css?family=Merriweather:400,700,400italic%7c" rel="stylesheet">
<link href='http://fonts.googleapis.com/css?family=Poiret+One' rel='stylesheet' type='text/css'>
<link href='http://fonts.googleapis.com/css?family=Limelight' rel='stylesheet' type='text/css'>
<!-- Latest compiled and minified CSS -->
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.5/css/bootstrap.min.css">
<!-- Latest compiled and minified JavaScript -->
<script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.5/js/bootstrap.min.js"></script>
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/font-awesome/4.4.0/css/font-awesome.min.css">
<meta name="image:Background" content=""/>
<meta name="image:Map" content=""/>
<meta name="image:Body" content=""/>
<meta name="if:Show Jumbotron" content="1" />
<meta name="color:Jumbotron Header Color" content="#000000" />
<meta name="color:Jumbotron Background Color" content="#ececec" />
<meta name="color:Jumbotron Body Color" content="#444444" />
<meta name="color:Jumbotron Button Color" content="#000000" />
<meta name="text:Jumbo Header" content=""/>
<meta name="text:Jumbo Content" content=""/>
<meta name="if:Show Jumbotron Button" content="1" />
<meta name="text:Jumbotron Button Text" content="" />
<meta name="text:Jumbotron Button Link" content="" />
<meta name="if:Show Map" content="1" />
<style>
@media screen { 
	html,body,div,span,object,iframe,h1,h2,h3,h4,h5,h6,p,blockquote,pre,abbr,address,cite,code,del,dfn,em,img,ins,kbd,q,samp,small,strong,sub,sup,var,b,i,dl,dt,dd,ol,ul,li,fieldset,form,label,legend,table,caption,tbody,tfoot,thead,tr,th,td,article,aside,figure,footer,header,menu,nav,section,menu,time,mark,audio,video {margin:0;padding:0;border:0;outline:0;font-size:100%;vertical-align:baseline;background:transparent;-webkit-box-sizing:border-box;-moz-box-sizing:border-box;box-sizing:border-box;}
	body { font-family:'Helvetica Neue',Helvetica,Arial,sans-serif; -webkit-text-size-adjust:none; background-color:#FCFCFC; color:#444; background-image: url('{image:Body}'); background-size: cover; background-attachment:fixed; overflow-x:hidden; }
	/*body.Menu a[href*="menu"], body.Contact a[href*="contact"] { background-color:#e5b354; }*/
	.fancy { font-family: 'Poiret One', cursive; }
	header { width:20vw; width:20%; height:100vh; height:100%; background-color:#fff; background-size:cover; float:left; position:fixed; padding-left:40px; background-image:url('{image:Background}'); border-right: 5px solid rgba(0, 0, 0, 0.3); z-index:100; }
	header img { width:100%;margin:50px 0 35px -20px;color:{AccentColor}; }
	header h1 { color: #000; }
	header p { color:#ccc; }
	.jumbotron { margin-left:20vw; margin-left: 20%; padding: 20px 50px; background-color:{color:Jumbotron Background Color}; text-align:center; }
	.jumbotron h1 { font-family: 'Limelight', cursive; color: {color:Jumbotron Header Color};}
	.jumbotron p { color: {color:Jumbotron Body Color} ;}
	.jumbotron .btn { margin: 10px 0 0 0; }
	footer { display: block; position:absolute; left:0; padding-left:20vw; padding-left:20%; }
	small { padding:0 !important; }
	mark { font-style: italic; font-weight: 600; color:inherit; font-size:inherit; }
	.contact-info { width:100%; height:50px; display:block; position: absolute; bottom:0; left:0; text-align: center; }
	.contact-info-mobile { width:100%; height:50px; display: none; }
	.contact-info a, .contact-info-mobile a { color: rgba(0, 0, 0, 0.7); margin-right:20px; }
	section { width:80vw; width: 80%; height:100vh; height: 100%; float:right; padding:0 150px; }
	article { padding:50px 0; }
	article:first-of-type{padding-top:0}
	article ul { font:1em Merriweather,georgia,serif; padding-left: 100px; }
	nav { z-index:99; }
	nav ul { padding:0; list-style: none; position:relative; }
	nav ul li a { display: block; padding:5px 15px; color:#000; text-decoration: none; background-color:#F7D65D; border-top-left-radius:5px; border-bottom-left-radius:5px; -webkit-transition: all 0.2s; transition: all 0.2s;}
	nav ul li a:hover { color:#000; background-color:#BFE559;text-decoration:none; }
	nav ul li a:active { background-color:#e5b354; }
	h1, h2, h3, h4, h5, h6	{color:#000}
	h1 {font-size:5em;letter-spacing:-2px}
	h2 {font-size:3em;letter-spacing:-1px;padding:50px 50px 40px 50px;max-width:100%;text-align: left;font-weight:600;}
	h2 a { color: #000; text-decoration: none; }
	h3 {font-size:1.5em;}
	h4 {font-size:1.3em;}
	h5 {font-size:1.1em;}
	h6 {font-size:0.9em;}
	p {font:1em Merriweather,georgia,serif; line-height:1.7em; margin:10px 0 30px 0; font-weight:400; }
	article p { padding:0 50px; }
	.datehold{position:relative;}
	time{text-transform:uppercase;font-size:.9em;color:#999;padding:110px 50px 30px 50px;display:block;position:absolute;}
	blockquote {font:1.3em Merriweather,georgia,serif; line-height:1.6em;  font-weight:400;font-style:italic; quotes:"\201C""\201D""\2018""\2019";padding:50px 0 50px 80px;max-width:850px}
	blockquote:before {color:#ddd; content:open-quote; font-size:4em; line-height:.1em; margin-right:.25em; vertical-align:-.4em;}
	small {font:.7em 'Helvetica Neue',Helvetica,Arial,sans-serif;padding:20px 50px;text-transform:uppercase;}
	small a{color:#999;}
	ul, ol {padding:0 0 0 20px;}
	li {font-size:1em; line-height:1.7em; padding:10px 0;}
	a {color:#111;}
	a:hover {color:{AccentColor};}
	a:hover, a:active {outline:none;}
	.button{background-color:#999;display:inline-block;padding:5px 15px;color:#fff;border-radius:3px;margin:10px 50px;text-decoration:none;text-transform:uppercase;}
	.button:hover{background-color:#000;color:#fff;}
	.next{float:right;}
	.prev{float:left;}
	form {padding:20px 0;}
	input, textarea {padding:5px; width:66%; margin: 0 0 10px 0; border:2px solid #ddd; font-size:1em; line-height:1em; -webkit-appearance:none;}
	textarea {height:90px;}
	textarea:focus, input:focus {border:2px solid #48b54e; outline: none;}
	input.submit-button {width:100px;border: none; background:#bdc3c7; color:#fff; padding:9px 12px 10px 12px; line-height: 22px; border-radius: 6px; -webkit-transition:0.25s; -moz-transition:0.25s; transition:0.25s;}
	input.submit-button:hover {background:#48b54e;}
	label {display:block;padding-top:5px; font-size:1.1em; line-height:1.6em;}
	.error {color:#fb3a3a; float: none; }
	img {max-width:100%; height:auto; border:none;}
	iframe{ max-width:100%; }
	hr {border:none; font-size:1px; height:1px; background-color:#ddd; width:100%; clear:both;}
	.obar {padding:0 50px}
    .obar li {list-style-type:none;display:inline-block;font-size:.76em;font-weight:400;padding:0 2px;line-height:1em;text-transform:uppercase;}
    .lb,.rb{float:right;margin-left:10px;}
    
    
.message {
width: 100%;
height: 0px;
padding: 0px;
transition: all 300ms cubic-bezier(0.17, 0.04, 0.03, 0.94);
-webkit-transition: all 300ms cubic-bezier(0.17, 0.04, 0.03, 0.94);
overflow: hidden;
box-sizing: border-box;
  
}

#toggle {
  position:absolute;
  appearance:none;
  cursor:pointer;
  left:-100%;
  top:-100%;
}

#toggle + label {
  cursor:pointer;
  padding:10px;
  background: {color:Jumbotron Button Color};
width: 100px;
border-radius: 3px;
padding: 8px 10px;
color: #FFF;
line-height:20px;
font-size:14px;
text-align:center;
-webkit-font-smoothing: antialiased;
cursor: pointer;
margin: 20px auto 0 auto;
  transition:all 500ms ease;
  -webkit-transition: all 500ms ease;
}
#toggle + label:after {
  content:"Book now!" 
}

#toggle:checked ~ .message {
  height: 300px;
  padding:20px 0;
}

#toggle:checked ~ .container {
  margin-top: 250px;
}

#toggle:checked + label {
  background:#dd6149;
}

#toggle:checked + label:after {
  content:"Close"
}
				
}
@media screen and (max-width:1030px) { 
    	h1{font-size:3em}
}
@media screen and (max-width:900px) { 
    body { overflow-x:hidden; }
	header {width:100vw;width:100%;height:auto;float:none;position:relative;padding-bottom:1px;border:0;}
	header img { width:80%; margin:20px auto; }
	footer { padding-left: 0; }
	.jumbotron { margin-left:0; }
	.contact-info-mobile { display: block; }
	.contact-info { display:none; }
	/*h1 { font-size:2em; }
	h2 { font-size:2em; }*/
	small, article h2, article p, .obar{padding-left:20px;padding-right:20px;}
	time { padding-top:90px; padding-left:20px; }
	section { width:100vw;width:100%;height:auto;float:none;padding:0; }
	article { padding:50px 0; }
	nav { width:90%;height:50px}
	nav ul{ width:100%;margin:0;display:block;overflow:auto;}
	nav ul li {display:inline-block;text-align:center;font-size:.8em;padding:5px 10px 5px 0;}
	nav ul li a{ display:block; border-radius:5px; } 
	.lb,.rb{float:none;margin:10px;}
}
</style>
</head>
<body class="{block:PostTitle}{PostTitle}{/block:PostTitle}" >
<header>
  {block:ShowAvatar}
    <a href="/"><img src="{HeaderImage}" /></a> 
    {/block:ShowAvatar}
    <nav role="navigation" class="nav-collapse">
    <ul>
      <li><a href="/" class="fancy">Home</a></li>
      <li><a class="fancy" href="http://sweetescapebysarataylor.com/post/128441084123/menu">Menu</a></li>
      {block:Pages}
      <li><a href="{URL}" class="fancy {block:PostTitle}{PostTitle}{/block:PostTitle}">{Label}</a></li>
      {/block:Pages}
      <!-- {block:AskEnabled}
        <li><a href="/ask">{AskLabel}</a></li>
      {/block:AskEnabled} -->
    </ul>
    </nav>
    <div class="contact-info">
        <a href="https://www.facebook.com/sweetescapebysarataylor"><i class="fa fa-facebook-square fa-2x"></i></a>
        <a href="https://instagram.com/sweetescapeskincare/"><i class="fa fa-instagram fa-2x"></i></a>
    </div>
    <div class="contact-info-mobile">
    <a href="https://www.facebook.com/sweetescapebysarataylor"><i class="fa fa-facebook-square fa-2x"></i></a>
    <a href="https://instagram.com/sweetescapeskincare/"><i class="fa fa-instagram fa-2x"></i></a>
</div>
</header>
{block:IndexPage}
{block:IfShowJumbotron}
<div class="jumbotron">
  <h1>{text:Jumbo Header}</h1>
  <hr>
  <p>{text:Jumbo Content}</p>
  {block:IfShowJumbotronButton}
  <a href="{text:Jumbotron Button Link}"><button type="button" class="btn btn-info">{text:Jumbotron Button Text}</button></a>
  {/block:IfShowJumbotronButton}
</div>
{/block:IfShowJumbotron}
{/block:IndexPage}

<section>
{block:Posts}
    
    {block:Photo}
    <article itemscope itemtype="http://schema.org/Article">
    <figure>
    <a href="{Permalink}"><img src="{PhotoURL-1280}" alt="{PhotoAlt}" /></a>
    </figure>
    <div class="datehold">
    <!-- {block:Date}<time>{DayOfMonth} {Month} {Year}</time>{/block:Date} -->
	{block:Caption}{Caption}{/block:Caption}
	</div>
	<ul class="obar">
	<!-- {block:IndexPage}
	<li><a href="{Permalink}">Permalink</a></li> 
	{/block:IndexPage} -->
	{block:HasTags} 
	<li>TAGS: </li>
	{block:Tags}<li><a href="{TagURL}">{Tag}</a></li>{/block:Tags}
	{/block:HasTags}
	{block:Date}
	<li class="lb">{LikeButton color="grey"}</li>
    <li class="rb">{ReblogButton color="grey"}</li>
    {/block:Date}
	</ul>
	<!-- <div class="lb">{LikeButton color="grey"}</div><div class="rb">{ReblogButton color="grey"}</div> -->
	{/block:Photo}
    
    {block:Text}
	<article>
	{block:Title}
	<h2>{block:IndexPage}<a href="{Permalink}">{/block:IndexPage}{Title}{block:IndexPage}</a>{/block:IndexPage}</h2>
	{/block:Title}
	{block:Body}
	{Body}
	{/block:Body}
	<ul class="obar">
	<!-- {block:IndexPage}
	<li><a href="{Permalink}">Permalink</a></li> 
	{/block:IndexPage} -->
	{block:HasTags} 
	<li>TAGS: </li>
	{block:Tags}<li><a href="{TagURL}">{Tag}</a></li>{/block:Tags}
	{/block:HasTags}
	{block:Date}
	<li class="lb">{LikeButton color="grey"}</li>
    <li class="rb">{ReblogButton color="grey"}</li>
    {/block:Date}
	</ul>
	{/block:Text}
	
{/block:Posts}

<hr>
<center><small>Copyright 2015 © Sweet Escape by Sara Taylor. Website design by <a href="http://curtisthornton.tumblr.com">Curtis Thornton</a>. Based on the Tumblr theme <a href="http://forward-theme.tumblr.com">Forward</a>.</small></center>

<!-- {block:IndexPage}
	{block:Pagination}
	<article>
    {block:Pagination}
    <small>
        {block:PreviousPage}
        <a href="{PreviousPage}" class="button prev">Previous</a> 
        {/block:PreviousPage}
        {block:NextPage}
        <a href="{NextPage}" class="button next">Next</a>
        {/block:NextPage}
    </small>
    {/block:Pagination} -->
    </article>
    {block:IfShowMap}
    <footer>
    <a href="https://www.google.com/maps/place/12330+St+Andrews+Dr,+Oklahoma+City,+OK+73120/@35.596292,-97.5877008,17z/data=!4m2!3m1!1s0x87b21c98c2ae470d:0xb32ba40eaf2e4508"><img src="{image:Map}" width=100% /></a>
    </footer>
    {/block:IfShowMap}
{/block:IndexPage}

</section>

</body>
</html>
