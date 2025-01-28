# Lab 4 - Market Place Additional Functionality
### Due - Tuesday, February 4, 11:59pm

There is no assignment link. Please add the functionality below to the
MarketPlace project in your Lab3 repository.

<hr/>

For this assignment, you will practice with design and
[refactoring](https://refactoring.guru/refactoring); sorting using `Comparable`
or `Comparator`; and Java streams. 

*It is permissible to use an LLM to generate your test cases (and only your test
cases).*

## Requirements

### Sort a list of products by price

You will modify your Lab3 solution to provide the ability to sort a 
`List<Product>` by their price. It is up to you to determine where this
functionality will be implemented, i.e., in which class or method. 

To earn full credit, you must follow the guidelines below:

- You must use test driven design. However you design your solution, it must be
  easily testable.
- You  must provide appropriate unit tests for your solution.
- You must use either the `Comparable` or `Comparator` interface.

### Reduce the price of all clothing of a given size

You will modify your Lab3 solution to provide the ability to specify a size of
clothing and discount percentage and reduce the price for all `Clothing` objects
with the given size in a given `List<Product>` by the amount specified.

To earn full credit, you must follow the guidelines below:

- You must use test driven design. However you design your solution, it must be
  easily testable.
- You  must provide appropriate unit tests for your solution.
- You must use the [Stream API](https://docs.oracle.com/javase/8/docs/api/java/util/stream/Stream.html).

*Hint: you may add methods to multiple classes in the project.*

### Calculate the average warranty length

You will modify your Lab3 solution to provide the ability to calculate the
average length of warranty for all `Electronics` objects in a `List<Product>`. 

To earn full credit, you must follow the guidelines below:

- You must use test driven design. However you design your solution, it must be
  easily testable.
- You  must provide appropriate unit tests for your solution.
- You must use the [Stream API](https://docs.oracle.com/javase/8/docs/api/java/util/stream/Stream.html).

### REFLECTION.md

You will add a file REFLECTION.md to the top-level folder of your repository.
Your reflection must describe, at minimum, the following:

1. An overview of your revised design. Include a short description of additional
   classes or methods.
2. Did you try any design that didn't work as expected? If so, briefly describe
   the design and why it didn't work.
3. Did you use an LLM to assist with generating your test cases?
4. Describe how you determined that your test cases were sufficient (especially
   if you used an LLM to help you).
5. Describe any bugs you encountered while using the Streams API. 