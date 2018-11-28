<!DOCTYPE html>
<html>
<head>
<title>Search Box Example 2 - default placeholder text gets cleared on click</title>
<meta name="ROBOTS" content="NOINDEX, NOFOLLOW" />
<!-- JAVASCRIPT to clear search text when the field is clicked -->
<script type="text/javascript">
window.onload = function(){ 
	//Get submit button
	var submitbutton = document.getElementById("tfq");
	//Add listener to submit button
	if(submitbutton.addEventListener){
		submitbutton.addEventListener("click", function() {
			if (submitbutton.value == 'search'){//Customize this text string to whatever you want
				submitbutton.value = '';
			}
		});
	}
}
</script>
<!-- CSS styles for standard search box with placeholder text-->
<style type="text/css">
	#tfheader{
		background-color:rgb(75, 75, 180);
	}
	#tfnewsearch{
		margin-left: 300px;
		padding:10px;
        
	}
	.tftextinput2{
		margin: 0;
		padding: 5px 15px;
		font-family: Arial, Helvetica, sans-serif;
		font-size:14px;
		color:#666;
		border:1px solid #0076a3; border-right:0px;
		border-top-left-radius: 5px 5px;
		border-bottom-left-radius: 5px 5px;
	}
	.tfbutton2 {
		margin: 0;
		padding: 5px 7px;
		font-family: Arial, Helvetica, sans-serif;
		font-size:14px;
		font-weight:bold;
		outline: none;
		cursor: pointer;
		text-align: center;
		text-decoration: none;
		color: #ffffff;
		border: solid 1px #0076a3; border-right:0px;
		background: #0095cd;
		background: (linear, left top, left bottom, from(#00adee), to(#0078a5));
		background: -moz-linear-gradient(top,  #00adee,  #0078a5);
		border-top-right-radius: 5px 5px;
		border-bottom-right-radius: 5px 5px;
	}
	.tfbutton2:hover {
		text-decoration: none;
		background: #007ead;
		background: (linear, left top, left bottom, from(#0095cc), to(#00678e));
		background: -moz-linear-gradient(top,  #0095cc,  #00678e);
	}
	/* Fixes submit button height problem in Firefox */
	.tfbutton2::-moz-focus-inner {
	  border: 0;
	}
	.tfclear{
		clear:both;
	}
    .roza {
        color:white;font-family: sans-serif;float:right;margin-right: 140px;text-decoration: none;padding-top: 9px;
    }
    .ghora{
        color:white;font-family: sans-serif;float:right;margin-right: 140px;padding-top: 9px;
    }
    .badass {
        color:white;font-family: sans-serif;float:right;margin-right: 140px;padding-top: 9px;
    }
    .badass:hover{background-color:rgb(255, 0, 255);background-clip: content-box;}
    
    #black {text-decoration: none;color:azure;padding-top: 9px;}
    #black:hover{background-color:rgb(255, 0, 255);background-clip: content-box;}
    #yahoodisazish {
        text-decoration: none;color: azure;
    }
    #yahoodisazish:hover{background-color:rgb(255, 0, 255);background-clip: content-box;}
    #noplace {
        text-decoration: none;color: azure;
    }
    .box{width:2000px;height:1000px;clear:both;position:fixed;}
    .red{background-color:rgb(239, 244, 255);color:grey;}
     
    .back {width:410px;height:100px;margin-left:400px;float:center;margin-top:10px;position:absolute;border:1px solid rgb(218, 216, 216);border-radius:4px ;}
     .topbox {width:450px;height:90px;background-color:rgb(249, 251, 255);font-family: sans-serif;color:gray;font-size: 25px;}
     
   #baba {
       height:16px;float:center;
   }
   .textmodi {
       padding:25px;
   }
   .babu {width:450px;height:1000px;float:center; margin-left:401px;clear:both;  }
   .sabu {background-color:rgb(249,251,255)
;position:absolute;margin-top:115px;border:1px solid rgb(218, 216, 216);border-radius:4px ;}
   .yama {
       width:350px;height:1000px;position:absolute;float:right;border:1px solid rgb(218, 216, 216);border-radius:4px ;
    
   }
   .sama {
       background-color:rgb(249,251,255);
   }
   .express{width:350px;height:1000px;position:absolute;clear:both;}
   .news {background-color:rgb(249,251,255);border:1px solid rgb(218, 216, 216);border-radius:4px ;float:right;}
   .romeo {color:rgb(0, 0, 0);font-family: sans-serif;border:30px solid rgb(249,251,255);position:absolute;float:right;}
   #bilal {width:30px;height:30px;position:absolute;}
   .wekho{font-family:sans-serif;margin-left:25px;margin-top:300px;}
   .jaoudr {height:400;width:450px;position:relative;}
</style>
</head>
<body>
	<!-- HTML for SEARCH BAR -->
	<div id="tfheader"><a target="_blank" href="www.facebook.com"><img id="baba" src="facebook.jpg"></a>
		<form id="tfnewsearch" method="get" action="http://www.google.com"><span class="roza"><a id="black" href="www.facebook.com">Find friends</a></span>&nbsp;&nbsp;&nbsp;&nbsp;<span class="ghora"><a id="yahoodisazish" href="https://www.youtube.com">Home</a></span>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span class="badass"><a id="noplace" href="www.facebook.com">Rehan</a></span>
		        <input type="text" id="tfq" class="tftextinput2" name="q" size="21" maxlength="120" value="Search our website"><input type="submit" value=">" class="tfbutton2">
		</form>
		<div class="tfclear"></div>
    </div>
    <div class="box red"><span class="shomeo">Story</span><br><br><span  class="dhomio">Add to your story</span></div>
    <div class="back topbox"><span class="textmodi">What's on your mind?</span></div>
    <div class="babu sabu"><img class="jaoudr" src="file:///C:/Users/Rehan/Documents/my%20website/pictureperfect.png">  </div>
    <div class="yama sama"></div>
    <div class="express news"></div>
    <div class="romeo">Stories<br><br>Add to your story<br><br>News feed<br><br><img id="bilal" src="sample.png"><span class="wekho"></span>messenger</div>
    
</body>
</html>

