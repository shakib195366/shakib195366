<!---FLOWPLAYER CODES STARTS HERE---->


<link href="//releases.flowplayer.org/7.2.5/skin/skin.css" rel="stylesheet"></link>


<link href="//demos.flowplayer.com/media/css/demo.css" rel="stylesheet"></link>


<link href="//demos.flowplayer.com/media/css/pygments.css" rel="stylesheet"></link>


<style>


.flowplayer {


  background-color: #333333;  height: 380px; width: 100%;


}


.flowplayer .fp-color-play {


  fill: #eee;


}


</style>


<script src="//code.jquery.com/jquery-1.12.4.min.js"></script>


<script src="https://cdnjs.cloudflare.com/ajax/libs/hls.js/0.8.9/hls.light.min.js"></script>


<script src="//releases.flowplayer.org/7.2.5/flowplayer.min.js"></script>


<br />




<div id="content">


<center>


Live streaming 1<br />


Just click the play button below to start watching the live stream.


</center>


<div class="flowplayer no-brand is-splash is-paused skin-custom fp-fat fp-outlined has-splash-text fp-default-playlist is-mouseout" data-live="true" data-ratio="0.4167" data-embed="false" data-ratio="0.5625" data-advance="false" data-qsel="-mobile,-mobile2,-sd,-md,-hd,-fullhd,-qhd,-4k" data-qlabels="240p,270p,360p,540p,720p,1080p,1440p,2160p">


<video data-title="Live stream">


<source src="https://rbmn-live.akamaized.net/hls/live/590964/BoRB-AT/master_3360.m3u8" type="application/x-mpegurl"></source></video>


</div>


</div>


<script>


if (location.search.indexOf("hlsjs=false") > -1) {


  flowplayer.conf.hlsjs = false;


} else if (location.search.indexOf("safari=true") > -1) {


  flowplayer.conf.hlsjs = {


    safari: true


  };


}


var toggleButton = document.getElementById("hlsjstoggle"),


    hlsjsLoaded = location.search.indexOf("hlsjs=false") < 0;


if (toggleButton) {


  if (flowplayer.engines[0].engineName !== "hlsjs") {


    toggleButton.parentNode.style.display = "none";


  } else {


    toggleButton.href = location.pathname + (hlsjsLoaded


      ? "?hlsjs=false"


      : "");


    toggleButton.getElementsByTagName("span")[0].innerHTML = hlsjsLoaded


      ? "without"


      : "with";


  }


}


</script>


<!---FLOWPLAYER CODES ENDS HERE---->
