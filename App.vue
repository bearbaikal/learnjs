/* eslint no-mixed-spaces-and-tabs: 0 */
<template>
	<div>
  	<h1>Hello, this is explonation for myself how to work with JS!</h1>
	  Let's start! There are several topics to play:
		<ul>
  		<li>
  			Arrays
  			<ul>
  				<li>
  					Examples presented in console (use F12 to open it here in Chrome)<br>
  					Look at source .vue file of this project between tags "script" to realize how it works
					</li>
  				<li>
  					split() method in JS works consequentially<br>
  					What does it mean?<br>
	  				When start working with arrays in JS you can stuck with one question - "How to put in array element with entire index?"<br>
	  				Despite your desire to specify random index with splice() method for array, you cannot do it!<br>
	  				In Example #1 i tried to specify random indexes for array, but elements get consequentially indexes
  				</li>
					<li>
						How to use splice method examples:
						<div>
							https://flaviocopes.com/how-to-add-item-to-array-javascript/#:~:text=You%20want%20to%20explicitly%20add,()%20method%20of%20an%20array.
						</div>
					</li>
				</ul>
			</li>
			<li>
				Eslint
				<div>
					The hot question in vue cli projects, including nuxt is how to disable eslint for period of development.<br>
					That's what i found for solve this:<br>
					<ul>
						<li>
							Add to root of project file with name .eslintignore and add one string with symbol *<br>
							It says eslint to stop checking all the files in project.<br>
							Note: plus of this method is it is possible to use it with instant prototiping with command "vue serve"
						</li>
						<li>
							Comment string '@nuxtjs/eslint-module' in buildModules section of nuxt.config.js file<br>
							Note: it's for nuxt projects compiled with eslint support
						</li>
					</ul>	
				</div>
			</li>
		</ul>
	</div>
</template>
<script>
	console.log("Hi! Code examples are below:")
	console.log("Example #1: add element to array with specified index")
	let arr = []
	console.log(arr)
	arr.splice(0, 0, 1)
	arr.splice(4, 0, 4)
	arr.splice(9, 0, 9)
	console.log(arr)
</script>