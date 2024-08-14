# Test Driven Development Interview Question Drills

- Can you explain the concept of Test-Driven Development (TDD)?
- What are the three main steps in the TDD cycle?
- How does TDD help in improving code quality?
- When writing tests first, how do you decide on what test to write initially?
- Can you describe the difference between unit tests and integration tests?
- How do you handle refactoring while following TDD?
- What are some challenges you’ve faced when practicing TDD?
- How do you know when to stop writing tests for a feature?
- Can you explain the importance of writing small, incremental tests in TDD?
- How would you approach testing a function with external dependencies (like a database) in TDD?
- How do you ensure your tests are reliable and not brittle?
- Can you give an example of how you’ve used TDD in a recent project?
- How does TDD influence the design of your code?
- What do you do when you find it difficult to write a test for a piece of code?
- How would you test a feature that involves asynchronous operations using TDD?
- Can you explain the concept of "mocking" in the context of TDD?
- How do you deal with legacy code when trying to introduce TDD practices?
- Can you discuss a situation where TDD might not be the best approach?
- How do you handle edge cases in TDD?
- How do you balance between writing comprehensive tests and maintaining development speed?
- How do you ensure that your tests cover both happy paths and edge cases?
- Can you describe the role of continuous integration (CI) in the context of TDD?
- How would you approach writing tests for a user interface (UI) component in TDD?
- What strategies do you use to manage test dependencies in TDD?
- How do you decide the level of granularity for your tests in TDD?
- Can you explain the difference between "test first" and "test after" development?
- How would you handle a scenario where a test is difficult to write or takes too long to run?
- What is your process for writing tests for code that interacts with third-party APIs?
- How do you measure the effectiveness of your tests in TDD?
- Can you describe a situation where you had to refactor your tests after a code change?
- How do you ensure that your test suite remains maintainable as your project grows?
- What is the role of code coverage in TDD, and how much coverage do you aim for?
- How do you handle situations where tests are passing, but the code doesn't work as expected in production?
- Can you discuss the trade-offs between writing comprehensive tests and keeping your test suite fast?
- How would you test a complex algorithm using TDD?
- What is your approach to testing code that relies on randomness or non-deterministic behavior?
- How do you incorporate feedback from failed tests into your development process?
- Can you explain how TDD fits into Agile or other iterative development methodologies?
- How do you handle tests that require complex setup or teardown procedures?
- How do you prioritize which tests to write first when starting a new feature in TDD?

### Experience Based Questions
- Can you walk me through a specific example of how you applied TDD to develop a feature from scratch?
- Describe a time when TDD helped you catch a bug early in the development process. What was the bug, and how did the test identify it?
- Can you share an example of a particularly challenging test you wrote while practicing TDD, and how you overcame that challenge?
- Talk about a time when following TDD led you to refactor your code. What changes did you make and why?
- Can you describe a situation where you wrote a test that was too broad or too specific? How did you adjust it?
- Discuss a scenario where TDD influenced your decision to change the design or architecture of your code.
- Can you provide an example of how you wrote tests for edge cases in a TDD process?
- Tell me about a project where TDD improved your confidence in the code you were writing. How did it impact your development process?
- Can you describe a situation where TDD helped you in writing modular, reusable code? Provide specific examples.
- Share an experience where you had to mock a dependency in your tests. How did it affect your development process?
- Discuss a time when your initial tests in TDD led you to discover issues with the initial design or require

### Code Snippets

## Question 1

Assume you’re practicing TDD and want to add a new feature to this function. 

```python
def calculate_discount(price, discount_rate):
    if discount_rate < 0 or discount_rate > 1:
        raise ValueError("Discount rate must be between 0 and 1.")
    return price - (price * discount_rate)
```

Let's say you need to add a feature where the discount cannot reduce the price below a certain minimum value, say £5. How would you modify the function and the tests? What tests would you write first, and how would they drive the changes to this code?

## Question 2

Here's a code snippet for a simple function:

```python
def is_palindrome(s):
    return s == s[::-1]
```

This function checks if a string is a palindrome (reads the same forward and backward). Imagine you’re using TDD and you’re asked to extend this function to ignore spaces and capitalization (e.g., "Race car" should be considered a palindrome). What tests would you write first, and how would you modify the function to make those tests pass?
