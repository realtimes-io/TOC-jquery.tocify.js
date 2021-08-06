# Zingfeng Fast Instruction

## Install

Base on jquery 3.6.0 + jquery UI 1.12.1 + bootstrap 3.3.7

- CSS

```HTML
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css">
<link rel="stylesheet" href="libs/jqueryui/jquery-ui.min.css">
<link href="../src/stylesheets/jquery.tocify.css" rel="stylesheet">
```

- JS

```HTML
<script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
<script src="../libs/jqueryui/jquery-ui.min.js"></script>
<script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js" ></script>
<script src="../src/javascripts/jquery.tocify.js"></script>
```

## Usage

HTML

```HTML
<div class="container">
     	<div class="row">
            <div class="col-md-3">
                <div id="toc"></div>
            </div>
            <div class="col-md-9">
                <div id="content">
                    <h1>Chapter 1: ....</h1>
                    <h2>1st Problem</h2>
                    <h3>Solution A</h3>
                    <h3>Solution B</h3>
                    <h3>Solution C</h3>

                    <h2>2nd Problem</h2>
                    <h3>Solution D</h3>
                    <h3>Solution E</h3>

                    <h1>Chapter 2: ....</h1>
                    <h2>1st Problem</h2>
                    <h3>Solution F</h3>
                    <h3>Solution G</h3>
                    <h3>Solution H</h3>
                </div>
            </div>
        </div>
    </div>	
```

JS

```javascript
var toc = $('#toc').tocify({
            context: "#content", // jquerySelector - The container element to generate the table of contents
            // 	default = "body"
            selectors: "h1,h2,h3,h4,h5", // The element's used to generate TOC. The order is important.
            ignoreSelector: "", // A selector to any element that would be matched by selectors that you wish to be ignored
        }).data("toc-tocify");	


```

## Demo

- demos/default_2021.html : Demo 2021

- demos/default-document.html: Demo old + detail doc

  

## Source

- src/