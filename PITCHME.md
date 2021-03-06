@title[abstraction]

The process of abstraction is the process of decomposition.

---

@title[abstraction_what_is_it]

We break a large, complex problem down into smaller, simpler problems, and then compose solutions to form an application.

---

@title[principle]

Software solutions should be decomposable into their component parts.

---

@title[principle]

Components can be recomponsed into new solutions without changing the internal component implementation details.

---

@title[forms]

Abstraction in software takes many forms:

* Algorithms
* Data structures
* Modules
* Classes
* Frameworks
* Functions

---
@title[characteristics_of_good_abstractions]

Characteristics of good abstractions:

* Simple
* Concise
* Reusable
* Independent
* Decomposable
* Recomposable

---

@title[functions]

Functions possess qualities that are essential for a good abstraction

---

@title[functions]

Identity — The ability to assign a name to it and reuse it in different contexts.

---

@title[functions]

Composition — The ability to compose simple functions to form more complex functions.

---

@title[pure_functions]

The most useful functions for abstraction in software are pure functions, which share modular characteristics with functions from math.
In math, a function given the same inputs will always return the same output.

---

@title[pure_functions_examples]

 It’s possible to see functions as relations between inputs and outputs. Given some input A, a function f will produce B as output

`f: A -> B`

`g: B -> C`


then exists `h: A -> C` which is really `A -> B -> C`. The complexity is hide without any effort.

---
@title[no_pure_functions]


Functions that are not pure might not have this property. If they change state somewhere else
then the function is not independent and cannot be used in different context.

---
@title[plan_composition]

Plan for composition. Write functions whose outputs will naturally work as inputs to many other functions. Keep function signatures as simple as possible.

---
@title[plan_composition]

Type-specific functions can’t be reused for data of a different type.
Lifting functions to work on many data types, or wrapping data to make it look like what the function is expecting make composition possible.

---

@title[inmutability]

One option to enforce the pureness of functions, is to not allow the mutation of state.

---
@title[inmutability_quote]

Immutability: The true constant is change. Mutation hides change. Hidden change manifests chaos. Therefore, the wise embrace history.

---
@title[inmutability_library]

For this we have libraries like inmutableJs and mori.
