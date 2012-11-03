<h1>HTML5 local storage</h1>
It helps a big deal with persistence storage, forget cookies or even sessions. Once you start using localStorage, you will never need cookies for persistence storage on the browser.
What HMTL5 local storage offers
	<ul>
	<li>Enough storage space for your browser interaction (default 5MB)</li>
	<li>It persists beyond page refresh. Data stored will remain even when you reboot your pc until you destroy or clear it.</li>
	<li>Stays on the client and only submitted to the server when you wish to.</li>
	</ul>
It uses named key/value pairs when storing data. All stored items are in string format. In the code below I used the JSON.stringify method of json2 method to convert all items before storage.

<h2>How to</h2>
It can be called in any of your pages like illustrated below. <br/> <a href="http://kedyr.wordpress.com/2012/09/27/multi-page-apps-and-amd-with-requirejs-backbonejs/">Check ou my artical on AMD, requirejs and Model loading.</a> 
```javascript
<script type="text/javascript">
require(["jquery","models/localstorage"], function($,Storage) {
	/** it can then be used like
		Storage.store(name,value);
		var topics = Storage.retrieve(name);
	*/
});
</script>
```