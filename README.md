# Ruby Getter Method Assignment Bug

This repository demonstrates a subtle bug in Ruby related to assigning values to the return of a getter method.  In Ruby, directly assigning a value to the result of a getter method does *not* modify the underlying instance variable.  This behavior can be unexpected for programmers accustomed to other languages where such assignments would mutate the object's state.

The `bug.rb` file contains code exhibiting this behavior. The `bugSolution.rb` file shows the correct approach to modifying instance variables.

## How to Reproduce

1. Clone this repository.
2. Run `ruby bug.rb`.  Observe that attempting to change the value via the getter does not alter the internal state.
3. Run `ruby bugSolution.rb` to see the corrected implementation.