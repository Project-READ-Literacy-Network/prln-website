+++
fragment = "config"

[[config]]
  type = "css" # Acceptable values are icon, meta, link, css, js. Default is empty. Would not add anything on empty.
  block = true # If set to true, would inject the code to the <head> tag. Default is false
  resource = "css/style.css" # Path to file, can be on page or in static/ directory. Default is empty.
    
[[config]]
  type = "js"
  html = """
  <script>
var nav = document.querySelector('.prln-nav');
nav.addEventListener('toggle', function (event) {
	// Only run if the prlnDD is open
	if (!event.target.open) return;
	// Get all other open prlnDDs and close them
	var prlnDDs = nav.querySelectorAll('.prlnDD[open]');
	Array.prototype.forEach.call(prlnDDs, function (prlnDD) {
		if (prlnDD === event.target) return;
		prlnDD.removeAttribute('open');
	});
}, true);
</script>
  """
  
[[config]]
  type = "js"
  html = """
<script>
function closeAboutDetails() {
  document.getElementById("aboutDetails").open = false;
}
</script>
  """
  
[[config]]
  type = "js"
  html = """
<script>
function closepSDetails() {
  document.getElementById("pSDetails").open = false;
}
</script>
  """
  
[[config]]
  type = "js"
  html = """
<script>
function closetRDetails() {
  document.getElementById("tRDetails").open = false;
}
</script>
  """
  
  
[[config]]
  type = "js"
  html = """
  <script>
var nav = document.querySelector('.prln-nav');
    window.addEventListener("wheel", () => {
    if (window.innerWidth>999){
	var prlnDDs = nav.querySelectorAll('.prlnDD[open]');
	Array.prototype.forEach.call(prlnDDs, function (prlnDD) {
		prlnDD.removeAttribute('open');
	});
    }
}, true);
</script>
  """

[[config]]
  type = "js"
  html = """
  <script>
var nav = document.querySelector('.prln-nav');
    window.addEventListener("click", () => {
    if (window.innerWidth>999){
	var prlnDDs = nav.querySelectorAll('.prlnDD[open]');
	Array.prototype.forEach.call(prlnDDs, function (prlnDD) {
		prlnDD.removeAttribute('open');
	});
    }
}, true);
</script>
  """

[[config]]
  type = "js"
  html = """
  <script>
var all_links = document.querySelectorAll('a');
for (var i = 0; i < all_links.length; i++){
       var a = all_links[i];
       if(a.hostname != location.hostname) {
               a.rel = 'noopener';
               a.target = '_blank';
       }
}
</script>
  """    
    
+++

