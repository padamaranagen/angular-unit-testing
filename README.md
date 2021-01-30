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

