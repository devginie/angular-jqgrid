# angular-jqgrid
Directive module for free-jqgrid 4.13.0

## How to Use

First, make sure to add free-jqgrid 4.13.0 to your project, as explained in
[free fork of jqGrid's ReadMe](https://github.com/free-jqgrid/jqGrid/blob/master/README4.13.0.md) since we don't bundle
free-jqgrid for you.

Add 'angular-jqgrid' to the list of dependencies in your Angular.JS application:

```javascript
angular.module('myapp', [
  'ngMaterial',
  'ngMessages',
  // ...
  'angular-jqgrid'
]);
```

In your controller, create two variables to hold the dataset and jqGrid options:

```javascript
angular.module('myapp').controller('MyController', function($scope) {
  $scope.myData = [{"fieldName1" : "row1-col1", "fieldName2" : "row1-col2", "fieldName3" : "row1-col3"},
    {"fieldName1" : "row2-col1", "fieldName2" : "row2-col2", "fieldName3" : "row2-col3"}];
  $scope.myGridOptions = {
    colNames : ['columnName1', 'columnName2', 'columnName3'],
    colModel : [{ name : 'fieldName1'}, { name : 'fieldName2', align : 'center'}, { name : 'fieldName3', align : 'center'}]
  };
```
    
