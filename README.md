# Angular-DLmenu
An Angular JS directive that wraps ResponsiveMultiLevelMenu Plugin by Codrops

### Usage:

```html
 <div ng-controller="TreeController">
    <tree family="data"></tree>
 </div>
  ```
  
    - The 'tree' directive is what generates the MultiLevel Menu.
    - 'data' here refers to the name of the scope variable that contains the data with which to populate the nenu

    - 'data' is of the following form 

#####Example:  To represent the following structure
```
    |
    - Fashion
    |    |
    |    - Men
    |    |    |
    |    |    - Shirts
    |    |    - Jackets
    |    |    - Jeans
    |    |
    |    - Women
    |         |
    |         - Dresses
    |         - Knits
    |         - Blouses
    |        
    - Design
         |
         - Men
         |    |
         |    - Shirts
         |    - Jackets
         |    - Jeans
         |
         - Women
               |
              - Dresses
              - Knits
              - Blouses
```

##### The following object is assigned as $scope.data:

```
    [{
        name : "Fashion",
        children: [{
            name : "Men",
            children: [{
                name : "Shirts",
                children: []
            },{
                name : "Jackets",
                children: []
            },{
                name : "Jeans",
                children: []
            }]
        },
        {
            name : "Women",
            children: [{
                name : "Dresses",
                children: []
            },{
                name : "Knits",
                children: []
            },{
                name : "Blouses",
                children: []
            }]
        }]
    },
    {
        name : "Design",
        children: [{
            name : "Men",
            children: [{
                name : "Shirts",
                children: []
            },{
                name : "Jackets",
                children: []
            },{
                name : "Jeans",
                children: []
            }]
        }, {
            name : "Women",
            children: [{
                name : "Dresses",
                children: []
            },{
                name : "Knits",
                children: []
            },{
                name : "Blouses",
                children: []
            }]
        }]
    }];
```
