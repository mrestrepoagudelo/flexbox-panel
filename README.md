<h1> Panel Flexbox </h1>
Panel made with flexbox

Example available at https://mrestrepoagudelo.github.io/flexbox-panel/

<h3>Include PanelFlexbox CSS:</h4>

```html
  <link href="m-panel.css" rel="stylesheet">
```

<h3>Example:</h4>

```html
<div class="m-panel" style="width: 500px; height: 500px;">
  <div class="m-header"><a class="m-title">Title</a></div>
  
  <div class="m-body">
    <div style="height: 800px;">body content</div>
  </div>
	
  <div class="m-footer">
    <div>Footer content</div>
  </div>
</div>
```

<h3>CSS:</h4>

```css
.m-panel{
	display: -webkit-box;      /* OLD - iOS 6-, Safari 3.1-6 */
	display: -moz-box;         /* OLD - Firefox 19- (buggy but mostly works) */
	display: -ms-flexbox;      /* TWEENER - IE 10 */
	display: -webkit-flex;     /* NEW - Chrome */
	display: flex;             /* NEW, Spec - Opera 12.1, Firefox 20+ */
	
	-webkit-flex-direction: column;
	-moz-flex-direction: column;
	-ms-flex-direction: column;	
	flex-direction: column;
	-webkit-box-orient: vertical;
	-moz-box-orient: vertical;
	-ms-box-orient: vertical;
	box-orient: vertical;
  	
	overflow: hidden;
	height: 100%;
	width: 100%;
	  
	-webkit-box-shadow: 0 2px 2px 0 rgba(0,0,0,0.14), 0 3px 1px -2px rgba(0,0,0,0.12), 0 1px 5px 0 rgba(0,0,0,0.2);
	box-shadow: 0 2px 2px 0 rgba(0,0,0,0.14), 0 3px 1px -2px rgba(0,0,0,0.12), 0 1px 5px 0 rgba(0,0,0,0.2);
}

.m-header{
	-webkit-box-flex: 0 0 auto;      /* OLD - iOS 6-, Safari 3.1-6 */
	-moz-box-flex: 0 0 auto;         /* OLD - Firefox 19- */
	-webkit-flex: 0 0 auto;          /* Chrome */
	-ms-flex: 0 0 auto;              /* IE 10 */
	flex: 0 0 auto;           

	-webkit-box-ordinal-group: 1;   /* OLD - iOS 6-, Safari 3.1-6 */
	-moz-box-ordinal-group: 1;      /* OLD - Firefox 19- */
	-ms-flex-order: 1;              /* TWEENER - IE 10 */
	-webkit-order: 1;               /* NEW - Chrome */
	order: 1;                       /* NEW, Spec - Opera 12.1, Firefox 20+ */

	overflow: auto;
	background-color: #f2f3fb;
}

.m-title{
	font-family: -apple-system,BlinkMacSystemFont,"Segoe UI",Roboto,Oxygen-Sans,Ubuntu,Cantarell,"Helvetica Neue",sans-serif;
	font-size: 1.25rem;
	line-height: 3;
	margin-left: 20px;
}

.m-body{
	-webkit-box-flex: 1 1;      	/* OLD - iOS 6-, Safari 3.1-6 */
	-moz-box-flex: 1 1;         	/* OLD - Firefox 19- */
	-webkit-flex: 1 1;          	/* Chrome */
	-ms-flex: 1 1;              	/* IE 10 */
	flex: 1 1;  					/* NEW, Spec - Opera 12.1, Firefox 20+ */

	-webkit-box-ordinal-group: 2;   /* OLD - iOS 6-, Safari 3.1-6 */
	-moz-box-ordinal-group: 2;      /* OLD - Firefox 19- */
	-ms-flex-order: 2;              /* TWEENER - IE 10 */
	-webkit-order: 2;               /* NEW - Chrome */
	order: 2;                       /* NEW, Spec - Opera 12.1, Firefox 20+ */ 

	overflow: auto;
}

.m-footer{
	-webkit-box-flex: 0 0 auto;      /* OLD - iOS 6-, Safari 3.1-6 */
	-moz-box-flex: 0 0 auto;         /* OLD - Firefox 19- */
	-webkit-flex: 0 0 auto;          /* Chrome */
	-ms-flex: 0 0 auto;              /* IE 10 */
	flex: 0 0 auto;           		/* NEW, Spec - Opera 12.1, Firefox 20+ */

	-webkit-box-ordinal-group: 3;   /* OLD - iOS 6-, Safari 3.1-6 */
	-moz-box-ordinal-group: 3;      /* OLD - Firefox 19- */
	-ms-flex-order: 3;              /* TWEENER - IE 10 */
	-webkit-order: 3;               /* NEW - Chrome */
	order: 3;   					/* NEW, Spec - Opera 12.1, Firefox 20+ */ 

	overflow: auto;
	border-top: 1px solid lightgray;
	background-color: #f2f3fb ;
}
```


