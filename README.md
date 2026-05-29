# Studio 4

## Functions and Operators

In this studio, you will explore how operators and functions can be used to compare and modify the state of variables, using the `Pressure` and `Weekday` enumerated types from Studio 2. You will examine operator precedence, use implicit conversion to compare enum values with `<`, and apply standard-library sets, iterators, and algorithms to compute intersections and unions of `Weekday` values.

## Collaboration

You may complete this studio individually or in a small group.

## Reference

If you need a refresher on the environment setup steps from the previous studios, see [Studio 0](https://github.com/cse4208-wustl/studio0).

If you need to review the `Pressure` and `Weekday` types and operators from earlier work, see [Studio 2](https://github.com/cse4208-wustl/studio2).

## Exercises

Record your answers in `ANSWERS.md` as you work. Include the names of everyone who worked on the studio in your first answer, and number your responses so they are easy to match to the exercises.

1. List the names of the people who worked together on this studio.

2. SSH into `shell.cec.wustl.edu` using your WUSTL Key credentials, then use `qlogin` to log into one of the Linux Lab machines and confirm that the version of `g++` there is correct, as you did in [Studio 0](https://github.com/cse4208-wustl/studio0).

   Clone your `studio4` repo and work inside that cloned directory.

   Add the header and source files from your completed Studio 2 work that declare and define the `Pressure` type and its operators.

   Define a `main` function for your program, and in it declare a variable of the `Pressure` enumerated type initialized to one of the enumerated values. Then write statements involving expressions that use both the shift operator with `cout` and the prefix increment operator you wrote for that type in Studio 2 to demonstrate which of those operators has higher precedence.

   Compile and run your program. In your answers, show:

   - the code you wrote for this exercise
   - the output your program produced
   - which of the operators has higher precedence
   - why the output demonstrates that precedence

3. Add the header and source files from your completed Studio 2 work that declare and define the `Weekday` type and its operators.

   In the `main` function for your program, declare additional variables of the `Pressure` and `Weekday` enumerated types initialized to different enumerated values than the ones you used previously.

   Without writing a specific less-than operator, `operator<`, for either type, write statements that use the built-in `<` operator and print output to `cout` demonstrating that the operator works correctly for comparisons of `Pressure` variables and for comparisons of `Weekday` variables.

   Compile and run your program. In your answers, show:

   - the code you wrote for this exercise
   - the output your program produced
   - why the output reflects correct behavior of the operator in each case

4. At the top of your main source file, or in a header file that it includes, add the standard `<set>` library header.

   In your main program, declare two `set` associative container objects for `Weekday` values and initialize or insert different values into them. Then iterate through each container and print the values that it contains.

   Compile and run your program. In your answers, show:

   - the code you wrote for this exercise
   - the output your program produced

5. At the top of your main source file, or in a header file that it includes, add the standard `<algorithm>` and `<iterator>` library headers.

   In your main program, declare another `set` object for `Weekday` values.

   Call the standard `set_intersection` function template with `begin()` and `end()` iterators for the `set` objects from the previous exercise, and a standard `inserter` initialized with the new `set` object and that object's `end()` iterator.

   Then iterate through the new `set` object and print the values that it contains, which should be the intersection of the other two sets.

   Compile and run your program. In your answers, show:

   - the code you wrote for this exercise
   - the output your program produced

6. In your main program, declare another associative container object for a different `set` of `Weekday` values.

   Call the standard `set_union` function template with `begin()` and `end()` iterators for the original `set` objects, and a standard `inserter` initialized with the new `set` object and that object's `end()` iterator.

   Then iterate through the new `set` object and print the values that it contains, which should be the union of the other two sets.

   Compile and run your program. In your answers, show:

   - the code you wrote for this exercise
   - the output your program produced

## Deliverables

Commit and push all modified and added files to the repo.

## Notes

- The original Studio 4 page told students to create a fresh course subdirectory and upload a text file to Canvas. Those workflow instructions were removed so the repo can serve as the assignment source of truth.
- This source material assumes students already completed Studio 2. This repo therefore expects students to bring forward their own `Pressure` and `Weekday` files from that work rather than publishing prior-studio solution code here.
