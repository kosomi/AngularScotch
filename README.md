# AngularScotch



<img src='https://github.com/kosomi/AngularScotch/blob/master/112123.png?raw=true'>

<img src='https://scotch.io/wp-content/uploads/2014/03/angular-routing-ui-router.jpg'>

0. Instruction: https://scotch.io/tutorials/angular-routing-using-ui-router


1. bower install angular-ui-router

1.  script src="bower_components/angular-ui-router/release/angular-ui-router.js"

1.  div ui-view


2. var app = angular.module('myApp', ['ngCordova', 'ui.router']);


3. app.config(['$stateProvider', '$urlRouterProvider', function($stateProvider, $urlRouterProvider) {
  $stateProvider
    .state('tab', {
      url: '/tab',
      abstract: true,
      templateUrl: 'templates/tabs.html'
    })
  $urlRouterProvider.otherwise('/tab/find');
}]);
