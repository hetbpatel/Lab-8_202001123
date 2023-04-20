# IT 314 - Software Engineering 
# Lab-8 : Unit Testing with JUnit
## Name - Het Patel
## ID - 202001123

## 1. Creating a new Eclipse project, package and defining the class
In Eclipse, a new Java project called Lab8 and a package inside it called mypackage is there.

![1](https://user-images.githubusercontent.com/124247624/233323808-71f472c5-4dcd-4efe-9b7a-cddd8d301b22.png)

### 2. Test method to test the behaviour of the Boa class : 

A class named Boa with the given code inside it.

![2](https://user-images.githubusercontent.com/124247624/233324392-f764ac0f-60a9-4229-b892-857e038f9ca8.png)

</br>

### 3. Modified setUp() method in the BoaTest class : 

created a JUnit test file for the Boa Class with name BoaTest

![3](https://user-images.githubusercontent.com/124247624/233325268-80cf401b-a02a-4ba4-81b6-15142b7d5df8.png)

</br>

### 4. Modified testIsHealthy() method in the BoaTest class : 
```
@Test
public void testIsHealthy() {
    // check that jen is not healthy
    assertFalse(jen.isHealthy());
    
    // check that ken is healthy
    assertTrue(ken.isHealthy());
}
```
</br>

### 5. Modified testFitsInCage() method in the BoaTest class : 

Implemented tests for the given two functions testIsHealthy() and testFitsInCage()

![4](https://user-images.githubusercontent.com/124247624/233325777-5eb93c31-d078-4cf7-9508-e8a977d666eb.png)

</br>

### 6. Running test cases:

![5](https://user-images.githubusercontent.com/124247624/233326147-2f4ecb0c-92c7-4926-8f84-12197a585601.png)

### 7. Here's the modified Boa class with the new lengthInInches() method:


![6](https://user-images.githubusercontent.com/124247624/233326599-bb70df5f-eb4a-4212-9a25-ae1adc3563ae.png)

</br>

### Adding new test cases to test lengthInInches()
    @Test
    public void testlengthInInches() {
    	assertEquals("error in lengthInInches()",  36, ken.lengthInInches());
    	assertNotEquals("error in lengthInInches()",  35, ken.lengthInInches());
        
    	assertEquals("error in lengthInInches()",  24, jen.lengthInInches());
    	assertNotEquals("error in lengthInInches()",  30, jen.lengthInInches());
    }

</br>

### Running the new Test Case


<img src="https://user-images.githubusercontent.com/95064151/233043180-b2f14800-de7b-4d43-a372-2e3cfdc44d44.png">
</br>
