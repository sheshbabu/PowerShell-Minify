PowerShell Minify
=================

A set of simple PowerShell scripts to combine/minfy JavaScript and CSS files.

Requirements
---------------

[YUI Compressor](http://yuilibrary.com/download/yuicompressor/)

[Closure Compiler](https://developers.google.com/closure/compiler/)

Getting started
---------------

### For CSS:

1) Open `Minify-CSS.ps1` and customize the paths

	$javaPath = "C:\Program Files\Java\jre6\bin\java.exe";
	$yuiPath  = "D:\lib\yui-compressor\yuicompressor-2.4.7\build\yuicompressor-2.4.7.jar"; 

	
2) Specify a output path for the minified file

	$outputPath = "D:\Output\yourfile-min.css";
	
3) Specify the paths for the source files that need to be minified

	$files = 
	"D:\Repository\source1.css",
	"D:\Repository\source2.css",
	"D:\Repository\source3.css"
	
4) Run the `Minify-CSS.ps1` script.

### For JavaScript:

1) Open `Minify-JS.ps1` and customize the paths

	$javaPath    = "C:\Program Files\Java\jre6\bin\java.exe";
	$closurePath = "D:\lib\closure-compiler\compiler.jar";
	
2) Specify a output path for the combined and minified files

	$combinedOutputPath = "D:\Output\yourfile-combined.js";
	$minifiedOutputPath = "D:\Output\yourfile-min.js";
	
3) Specify the paths for the source files that need to be minified

	$files =
	"D:\Repository\source1.js",
	"D:\Repository\source2.js",
	"D:\Repository\source3.js"
	
4) Run the `Minify-JS.ps1` script.

