PhantomJS-Jasmine
=================

Simple phantom script to run jasmine tests.

This is a phantom script that is derived from the jasmine example on phantomjs site. There were bugs in it so I re-wrote the example to work with Jasmine 2.0.0.

Download the script, and throw run-jasmine.js into the directory that runs your SpecRunner.html file. You can actually place it anywhere you want and use a relative path name. You still need SpecRunner.html to work. Such a file will look similar to what is bellow:

SpecRunner.html


<!DOCTYPE HTML>
<html>
<head>
  <meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
  <title>Jasmine Spec Runner v2.0.0</title>

  <link rel="shortcut icon" type="image/png" href="lib/jasmine-2.0.0/jasmine_favicon.png">
  <link rel="stylesheet" type="text/css" href="lib/jasmine-2.0.0/jasmine.css">

  <script type="text/javascript" src="lib/jasmine-2.0.0/jasmine.js"></script>
  <script type="text/javascript" src="lib/jasmine-2.0.0/jasmine-html.js"></script>
  <script type="text/javascript" src="lib/jasmine-2.0.0/boot.js"></script>

  <!-- include source files here... -->
  <script type="text/javascript" src="src/hello.js"></script>

  <!-- include spec files here... -->
  <script type="text/javascript" src="spec/hello.js"></script>

</head>

<body>
</body>
</html>

Once you have your SpecRunner.html setup, simply run it with phantomjs using the following command:

phantomjs run-jasmine.js SpecRunner.html

On a side note, you don't have to name you file SpecRunner.html. It can be called anything you want such as testFile.html.

phantomjs run-jasmine.js testFile.html

or

phantomjs run-jasmine.js path/to/RandomSpecRunningFile.html

phantomjs run-jasmine.js [relative path to file]

Enjoy!
