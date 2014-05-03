## Files to get started with Angular

index.html

  <!DOCTYPE html>
  <html ng-app="plunker">
  
    <head>
      <meta charset="utf-8" />
      <title>AngularJS Plunker</title>
      <script>document.write('<base href="' + document.location + '" />');</script>
      <link rel="stylesheet" href="style.css" />
      <script data-require="angular.js@1.2.x" src="https://code.angularjs.org/1.2.16/angular.js" data-semver="1.2.16"></script>
      <script src="app.js"></script>
    </head>
  
    <body ng-controller="MainCtrl">
      <p>Hello {{name}}!</p>
    </body>
  
  </html>

app.js

  var app = angular.module('plunker', []);

  app.controller('MainCtrl', function($scope) {
    $scope.name = 'World';
  });

style.css

  /* Put your css in here */

