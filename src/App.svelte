<script>
	import Nav from './Nav.svelte';
	import { Router, Route } from "svelte-navigator";
</script>


<Router>
	<Nav />
	<Route path="/">
		<div class="row">
			<div class="side">
				<h2>About Me</h2>
				<h5>Photo of me:</h5>
				<div class="fakeimg" style="height:200px; background: black; color: #FFD405">Use right and left arrows to see other scroll effects</div>
				<p>Some text about me in culpa qui officia deserunt mollit anim..</p>
				<h3>More Text</h3>
				<p>Lorem ipsum dolor sit ame.</p>
				<div class="fakeimg" style="height:60px;">Image</div><br>
				<div class="fakeimg" style="height:60px;">Image</div><br>
				<div class="fakeimg" style="height:60px;">Image</div>
			</div>
			<div class="main">
				<h2>TITLE HEADING</h2>
				<h5>Title description, Dec 7, 2017</h5>
				<div class="fakeimg" style="height:200px;">Image</div>
				<p>Some text..</p>
				<p>Sunt in culpa qui officia deserunt mollit anim id est laborum consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco.</p>
				<br>
				<h2>TITLE HEADING</h2>
				<h5>Title description, Sep 2, 2017</h5>
				<div class="fakeimg" style="height:200px;">Image</div>
				<p>Some text..</p>
				<p>Sunt in culpa qui officia deserunt mollit anim id est laborum consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco.</p>
			</div>
		</div>
	</Route>

	<Route path="about">
		<h3>About</h3>
		<p>That's what it's all about!</p>
	</Route>
</Router>

<div class="footer">
	<h2>Footer</h2>
</div>

<style>
* {
  box-sizing: border-box;
}


/* Column container */
.row {  
  display: -ms-flexbox; /* IE10 */
  display: flex;
  -ms-flex-wrap: wrap; /* IE10 */
  flex-wrap: wrap;
	padding-top: 5%;
}

/* Create two unequal columns that sits next to each other */
/* Sidebar/left column */
.side {
  -ms-flex: 30%; /* IE10 */
  flex: 30%;
  background-color: #f1f1f1;
  padding: 20px;
}

/* Main column */
.main {   
  -ms-flex: 70%; /* IE10 */
  flex: 70%;
  background-color: white;
  padding: 20px;
}
		

/* Fake image, just for this example */
.fakeimg {
  background-color: #aaa;
  width: 100%;
  padding: 20px;
}

/* Footer */
.footer {
  padding: 20px;
  text-align: center;
  background: #ddd;
}

/* Responsive layout - when the screen is less than 700px wide, make the two columns stack on top of each other instead of next to each other */
@media screen and (max-width: 700px) {
  .row {   
    flex-direction: column;
  }
}

/* Responsive layout - when the screen is less than 400px wide, make the navigation links stack on top of each other instead of next to each other */
@media screen and (max-width: 400px) {

}
</style>