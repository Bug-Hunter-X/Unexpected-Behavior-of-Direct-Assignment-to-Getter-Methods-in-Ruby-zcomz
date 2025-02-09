# Ruby Getter Method Assignment Bug

This repository demonstrates an uncommon yet potentially confusing bug in Ruby related to how getter methods interact with instance variable assignments.  Direct assignment to a getter method does not modify the underlying instance variable.

## The Problem

The `bug.rb` file contains code that illustrates the unexpected behavior.  While `instance_variable_set` correctly updates the instance variable, direct assignment to the getter method does not.

## The Solution

The `bugSolution.rb` file demonstrates a corrected approach using either a setter method or `instance_variable_set` for modifying instance variables.