# Angular-Unit-Testing

## unit testing for beginners
### 1. Unit Testing Fundamentals

* Small functions / methods ( 10 lines of code or less)
* Proper naming
* Single responsibility


Demo:

https://stackblitz.com/edit/1-fundamentals

### 2. Working with Strings and Arrays

*  Test should not be fragile

Demo: 

https://stackblitz.com/edit/2-working-with-strings-and-arrays

### 3. Setup and Tear down

Each test case should have 3 Asssss
* Arrange
* Act
* Assert
  
//Arrange
component = new AppComponent();

//Act
component.increament();

//Assert
expect(component.count).toBe(1);


Remember each test should test isolated work
 the solution to define a function as isolation is **beforeEach**
  similarly we have afterEach
  --you have to cleanup all in **afterEach** condition
 **beforeAll**
  **AfterAll**

 ` 
 beforeEach(() => {
    //Set up
  });
  afterEach(() => {
    //Tear Down
  });
`

Demo:

https://stackblitz.com/edit/3-setup-and-teardown

### 4. Working with Forms

Demo:

https://stackblitz.com/edit/4-working-with-forms

### 5. Working with Event Emitters

EventEmitters often we use @Output decorator in angular components.
EventEmitters are observeables, we can subscribe to them.

Demo:

https://stackblitz.com/edit/5-event-emitter


### 6. Working with Component,Service, Model and Mock

In Unit test, we don't want to touch the file system, database or callback of services. so we'll create a fake service, this won't make any backend or service calls. It will return a simple observable.


Demo:

https://stackblitz.com/edit/6-component-service-interaction


### 7. Interaction Testing -- adding --Inserting data

Demo:
