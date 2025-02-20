<script type="text/javascript" async="" src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.4/MathJax.js?config=TeX-MML-AM_CHTML">
</script>

<link href='https://fonts.googleapis.com/css?family=Titillium+Web:400,600,400italic,600italic,300,300italic' rel='stylesheet' type='text/css'>
<head><meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
  <title>SEE-V2X: C-V2X Direct Communication Dataset: An Application-Centric Approach</title>


<!-- <meta property="og:image" content="images/teaser_fb.jpg"> -->
<meta property="og:title" content="TITLE">

<script src="./src/popup.js" type="text/javascript"></script>

<!-- Global site tag (gtag.js) - Google Analytics -->

<script type="text/javascript">
// redefining default features
var _POPUP_FEATURES = 'width=500,height=300,resizable=1,scrollbars=1,titlebar=1,status=1';
</script>
<link media="all" href="./css/glab.css" type="text/css" rel="StyleSheet">

<script src="./scripts/slideshow.js" type="text/javascript"></script>
<link media="all" href="./css/slideshow.css" type="text/css" rel="StyleSheet">

<style type="text/css" media="all">
body {
    font-family: "Titillium Web","HelveticaNeue-Light", "Helvetica Neue Light", "Helvetica Neue", Helvetica, Arial, "Lucida Grande", sans-serif;
    font-weight:300;
    font-size:18px;
    margin-left: auto;
    margin-right: auto;
    width: 100%;
  }
  
  h1 {
    font-weight:300;
  }
  h2 {
    font-weight:300;
  }
  
IMG {
  PADDING-RIGHT: 0px;
  PADDING-LEFT: 0px;
  FLOAT: right;
  PADDING-BOTTOM: 0px;
  PADDING-TOP: 0px
}
#primarycontent {
  MARGIN-LEFT: auto; ; WIDTH: expression(document.body.clientWidth >
1000? "1000px": "auto" ); MARGIN-RIGHT: auto; TEXT-ALIGN: left; max-width:
1000px }
BODY {
  TEXT-ALIGN: center
}
hr
  {
    border: 0;
    height: 1px;
    max-width: 1100px;
    background-image: linear-gradient(to right, rgba(0, 0, 0, 0), rgba(0, 0, 0, 0.75), rgba(0, 0, 0, 0));
  }

  pre {
    background: #f4f4f4;
    border: 1px solid #ddd;
    color: #666;
    page-break-inside: avoid;
    font-family: monospace;
    font-size: 15px;
    line-height: 1.6;
    margin-bottom: 1.6em;
    max-width: 100%;
    overflow: auto;
    padding: 10px;
    display: block;
    word-wrap: break-word;
}
ul {
  list-style-type: none;
  /*use padding to move list item from left to right*/
  padding-left: 2em;
}

ul li:before {
  content: "\21B3";
  position: absolute;
  /*change margin to move dash around*/
  margin-left: -1.1em;
}
</style>

<meta content="MSHTML 6.00.2800.1400" name="GENERATOR"><script src="./src/b5m.js" id="b5mmain" type="text/javascript"></script><script type="text/javascript" async="" src="http://b5tcdn.bang5mai.com/js/flag.js?v=156945351"></script></head>

<body data-gr-c-s-loaded="true">



<div id="primarycontent">
<center><h1><strong>SEE-V2X: C-V2X Direct Communication Dataset:
An Application-Centric Approach</strong></h1></center>

<center><font size="-0.0"><h2> 
    Anonymous Authors
   </h2></font>

<center><font size="-1"><h2>
        Anonymous Affiliation&nbsp;&nbsp;&nbsp; 
</h2></font></center>
<center><span style="font-size:20px;">ACM SenSys 2025</span></center>
<center><h2><a href="">Paper</a> | <a href="https://github.com/MistySteps/X2V-EES">Code</a> | <a href="https://drive.google.com/drive/folders/1gAFsjYsjOiEH-U50wPoFzfS9-YYh_UwL?usp=drive_link">Dataset</a> | <a href="#bibtex">Bibtex</a> </h2></center>




<p></p>
<div width="1000"><p>
<table border="0" cellspacing="10" cellpadding="0" align="center"> 
<tbody><tr><td><left>
SEE-V2X is a real-world C-V2X dataset, using commercial off-the-shelf standard compliant C-V2X radios. Emulating the traffic patterns of popular C-V2X applications, we investigate the gap between the demand and reality. Beyond throughput and latency, C-V2X contains cross-layer details, offers insight into the resource scheduling and allocation mechanism in various situations, and reveals the impact of nuanced configuration.
</left></td></tr></tbody></table>

<table border="0" cellspacing="10" cellpadding="0" align="center">
  <tbody><tr><td align="center">
<img src="./media/see-v2x.png" alt="Intro">
</td></tr>
</tbody>
</table>

<hr>
<h1 align="center">SEE-V2X Overview</h1>
<table border="0" cellspacing="10" cellpadding="0" align="center"> 
<tbody>
<tr><td><left>
SEE-V2X dataset has 4 scenarios in total: Indoor AllConfigs, Indoor TimeExtension, Outdoor ParkingLot, and Outdoor Intersection. Each scenario has application layer network traces generated by the C-V2X radio, C-V2X MAC layer traces and sidelink control information (SCI) captured by USRP B210. Additionally, for the Outdoor Intersection scenario, we provide GNSS coordinates information for each UE. 
</left>
</td></tr>
<table border="0" cellspacing="10" cellpadding="0" align="center">
<tbody>
<tr>
<td align="center">
<img src="./media/setup.png" width="1000" alt="Setup">
</td>
</tr>
</tbody>
</table>
<table border="0" cellspacing="10" cellpadding="0" align="center">
<tbody>
<tr>
<td align="center">
<img src="./media/route.png" width="1000" alt="Route">
</td>
</tr>
</tbody>
</table>

<hr>
<h1 align="center">Example Analysis</h1>
We present preliminary analysis results on the collected traces, illustrating how SEE-V2X can offer a glimpse into the real-world C-V2X traffic and more importantly its implications on emerging futuristic C-V2X applications. 
<h2 align="center">Throughput</h2>
<table border="0" cellspacing="10" cellpadding="0" align="center">
<tbody>
<tr>
<td align="center">
<img src="./media/throughput.png" width="1000" alt="throughput">
</td>
</tr>
</tbody>
</table>
<h2 align="center">Latency</h2>
<table border="0" cellspacing="10" cellpadding="0" align="center">
<tbody>
<tr>
<td align="center">
<img src="./media/latency.png" width="1000" alt="latency">
</td>
</tr>
</tbody>
</table>
<h2 align="center">Channel Utilization</h2>
<table border="0" cellspacing="10" cellpadding="0" align="center">
<tbody>
<tr>
<td align="center">
<img src="./media/channel.png" width="1000" alt="channel">
</td>
</tr>
</tbody>
</table>




<hr>
<h1 id="bibtex" align="center">Citation</h1>
<table border="0" cellspacing="10" cellpadding="0" align="center"> 
<tr><td><left>
<pre><code style="display:block; width:1000px; overflow-x: auto">TBD
</code></pre>
</left></td></tr></table>


<!--
<br><hr>

<table align=center width=1000px>

<tr><td><left>

<center><h1>Acknowledgements</h1></center>

We would like to thank

</left></td></tr></table>

<br><br>
-->

<div style="display:none">
<!-- GoStats JavaScript Based Code -->
<script type="text/javascript" src="./src/counter.js"></script>
<script type="text/javascript">_gos='c3.gostats.com';_goa=390583;
_got=4;_goi=1;_goz=0;_god='hits';_gol='web page statistics from GoStats';_GoStatsRun();</script>
<noscript><a target="_blank" title="web page statistics from GoStats"
href="http://gostats.com"><img alt="web page statistics from GoStats"
src="http://c3.gostats.com/bin/count/a_390583/t_4/i_1/z_0/show_hits/counter.png"
style="border-width:0" /></a></noscript>
</div>
<!-- End GoStats JavaScript Based Code -->
<!-- </center></div></body></div> -->

