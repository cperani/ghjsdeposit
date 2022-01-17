# ghjsdeposit
external js scripts for webflow site

webflow as of this writing 01.17.22 does not permit uploading of .js files.  The .js files may be referenced by using webflow's embed utility.

this method for fetching .js files from github is discussed here ...

https://discourse.webflow.com/t/host-script-and-use-it-in-webflow/120771/6


Vako_Shvili
Community Contributor

2
Feb '21
UPDATE: OK, this version is now correct.

I’ve uploaded the JS code externally. You can load it using this code:

<script type="text/javascript" src="https://cdnjs.cloudflare.com/ajax/libs/three.js/r125/three.min.js" ></script>
<script type="text/javascript" src="https://cdn.jsdelivr.net/gh/VolkerShmuley/interactive-particles/script.js"></script>
Paste this code in the body tag of the page. 18

Then you’ll need to copy the remaining HTML and CSS snippets from the codepen. HTML should go inside the custom code embed element 9.

CSS should go in the head tag using the previous page settings method. You’ll need to wrap the CSS between these tags:

<style>
 /* CSS code goes here */
</style>
I tried it. It works.

I am seeing now that I misinterpreted Vako's comments.  He asked the person that needed help to upload their project to github so he could test
his solution.  The external .js file is actually being hosted by jsdelivr.net not github.
