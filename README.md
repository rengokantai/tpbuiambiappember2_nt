# tpbuiambiappember2_nt
##2
###2 Build models
```
ember generate model calendar
```
###3
create
```
ember g model day
```
create route
```
ember g route new
```
and change in app/router.js
```
Router.map(function() {
  this.route('new',{path:'/calendars/new'});
});
```
and we can delete all files 
```
rm app/routes/new.js

rm app/templates/new.hbs

rm test/unit/routes/new-test.js
```
then regenerate
```
ember g route new --path=/calendars/new
```

start server
```
ember serve --proxy http://localhost:4300
```
###4
```
ember g controller new
```
####07:30
If route and controller define same function, the controller's function will be called.  
####07:43 seperate responsibility
manage the model from the controller and manage the transition from the route


