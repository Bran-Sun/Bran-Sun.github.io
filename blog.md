---
layout: page
title: Blog
---

Last Update Dec. 2019

## Z3 study notes

ref: https://rise4fun.com/z3/tutorial/guide

1. Declare
	* declare-const
	* declare-fun: (declare-fun f(Int Bool) Int)
2. Assert
	* adds formulas into Z3 internal stack
	* **satisfiable** if there is an interpretation that makes all asserted formulas true
3. Scope
	* Z3 maintains a global stack of declarations and assertions
	* push create a new stack from current stack size
4. define-sort
	* defines a new sort symbol that is for a sort expression.
	* examples: 1. define-sort Set (T) (Array T Bool)
