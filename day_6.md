# Day 6

```

// Your result will be shown as an unique line. I wrote it with 
// extra line breaks for disply purposes only.

// <div class="container">
//     <li><h2>Title One</h2><li>
//     <li><h2>Title Two</h2><li>
//     <li><h2>Title Three</h2><li>
//     <li><h2>Title Bess</h2><li>
// </div>


function createHtml(css, titles) {
	var result = '<div class="'+css+'">';
	var append;
	for (var i=0; i<titles.length; i++) {
		append = '<li><h2>'+titles[i]+'</h2></li>';
		result += append;
	}
	return result += '</div>';
}

console.log(createHtml('container', ['Title One', 'Title Two', 'Title Three', 'Title Bes']));

```
