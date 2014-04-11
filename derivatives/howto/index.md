---
layout: derivative
title: Publish your derivative
category: derivative
folder: howto
---
<br>

<!--
The page URLs should be like:
{{ site.baseurl }}derivatives/{{ page.folder }}/sub-folder/file.jpg

example:
{{ site.baseurl }}derivatives/{{ page.folder }}/images/rubber.jpg
-->
If you worked on your Primo derivative, you can publish it here very easily. <br>
We created a checklist to help you build a meaningful document that other people can use. 

###Tick all of them to see the next steps:

<input type="checkbox" id="derp1" checked/>
<label for="derp1">Make a Primo Derivative</label>
<input type="checkbox" id="derp2" />
<label for="derp2">Write a bill of materials with prices and URLs</label>
<input type="checkbox" id="derp3" />
<label for="derp3">Collect and organise all the design files</label>
<input type="checkbox" id="derp4" />
<label for="derp4">Write an understandable guide</label>
<input type="checkbox" id="derp5" />
<label for="derp5">Collect pictures during the process, select the most significative ones and give them meaningful names</label>
<input type="checkbox" id="derp6" />
<label for="derp6">Draw some sketches of parts that can be misinterpreted</label>
<input type="checkbox" id="derp7" />
<label for="derp7">Organise all the materials in meaningful sub-folders, like ("images", "schemes", "files", etc)</label>
<input type="checkbox" id="derp8" />
<label for="derp8">Include your contact information</label>
<input type="checkbox" id="derp9" />
<label for="derp9">Select a license for your work</label>

<div id="instructions" markdown="1">
<br>

##How to publish your documentation

1. **super easy, no automation:** <br>
Write a document with your materials and mail it to us at [play@primo.io](mailto:play@primo.io). Mind that if you do it this way, we will just publish the download link to your document. To avoid this, please make your document in Markdown or HTML, like a single page website

2. **medium, light automation** <br>
Create a single-page website (markdown is preferred, but HTML is fine too) with your documentation, organized in sub-folders for images and files. 
Then zip the folder and send it at [play@primo.io](mailto:play@primo.io)

3. **advanced, full automation** <br>
Start by making a single-page website in Markdown with all your documentation, organized in sub-folders for images and files.<br>
At the top of your main .md file, include a [YAML header](http://jekyllrb.com/docs/frontmatter/), with the following properties:<br>
<br>
---<br>
layout: derivative<br>
category: derivative<br>
title: My Derivative Title<br>
folder: folder-name<br>
---<br>
<br>
/* your content in markdown or HTML here */<br>
<br>
Then [fork the repository on GitHub](https://github.com/primo-io/prototype-documentation), all the derivatives are located in the 'derivatives' folder, each one in its own subfolder. 
Paste here your website folder (your folder's name must be the same as the "folder" properties you indicated in the YAML header), then create a pull request on GitHub, to merge your files.

</div>

<script src="http://code.jquery.com/jquery-latest.min.js"
        type="text/javascript"> </script>

<script type="text/javascript">
	$("#instructions").hide();

	$("input:checkbox").change(function() {
		if ($('input:checked').length == $('input:checkbox').length) {
			$("#instructions").show();			  		    		    
		    goToByScroll("instructions"); 
		} else {
			$("#instructions").hide();
		}
	});

	// This is a functions that scrolls to #{blah}link
	function goToByScroll(id) {				
		$('html,body').animate({
				scrollTop: $("#" + id).offset().top
			},
			'slow');
	}
</script>