# lecture-19-Part-4-ScopeAndInheritance
lecture-19-Part-4-Scope and Inheritance

# Date: Jan 13, 2017:
- Controller as a Syntax
- Inheritance in general is used for code re-use(and sometimes to express a relationship between entities).
- Prototypal inheritance in JS is based on object instances rather than classes.
	- Property in inherited from parent, looked up through Protoype Chain.
	- Property is local if its declared on the child with the same name as the parent and therefore masking the parent's property.
- $scope is based on prototypal inheritance.
	- Child controller's $scope inherits from parent controller's $scope.
- Controller As Syntax is ControllerName as label.
- Angular creates property 'label' on the $scope.
	- the label is a reference to 'this', i.e. instance of controller.
	- Works because .controller treats its as a function contructor.
- Attach properties to 'this' inside of controller, not $scope.
	- Easier syntax in HTML and JS - no masking occurs.
