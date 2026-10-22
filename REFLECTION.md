## Reflection

1. Why should the fields be private? To ensure data integrity and encapsulation, fields are made private. Internal state is concealed and direct modifications from outside of class which are either not authorized or not valid are not permitted. Rather, access is restricted using only public getters and setters which validate the property.

3. What happens if the Car constructor does not call super(...)? If the Car constructor does not call super(...), Java will try to call the default constructor (no-argument constructor) of the parent class (super()). Note that the Vehicle class has a constructor that takes two arguments, so there is no default constructor (no arguments), which will cause a compilation error.

4. What is the difference between this.type and super.type? “this.type” is the same variable as it was in the parent class, but is shadowed by the variable defined in the current class. ”super.type” is a different variable that explicitly refers to the variable defined in the parent class.
