# 1.1 Propositions and Logical Operations

**Logic** - reasoning conducted or assessed according to strict principles of validity<br>
**Proposition** - a statement that is either true or false

✅ Examples of propositions:

- There are an infinite number of prime numbers. --> TRUE
- 17 is an even number. --> FALSE

❌ NOT propositions:

- What time is it? // A question is neither true nor false
- Are you awake? // Yes/No questions are neither true nor false
- Have a nice day. // A command is neither true nor false

**Truth value** - a value indicating whether the proposition is true or false<br>
A proposition is still a proposition whether its truth value is known to be _true, false, unknown, or a matter of opinion_

Examples of propositions and their truth values:

- Two plus two is four. --> TRUE
- Two plus two is five. --> FALSE
- Monday will be cloudy. --> UNKNOWN
- The movie was funny. --> MATTER OF OPINION

Propositional variables such as _p, q,_ and _r_ are used to denote arbitrary propositions, as in:

> **_p_**: January has 31 days.  
> **_q_**: February has 33 days.

**Compound proposition** - created by connecting individual propositions with logical operators<br>
**Logical operation** - combines propositions using a particular composition rule

### The Conjunction Operation (∧)

The proposition **_p_** ∧ **_q_** is read "**_p_** and **_q_**" and is called the **conjunction** of **_p_** and **_q_**.

> **_p_** ∧ **_q_** is TRUE if both **_p_** is true and **_q_** is true  
> **_p_** ∧ **_q_** is FALSE if **_p_** is false, **_q_** is false, or both are false

```
Truth Table: CONJUNCTION (∧)

 p     q       p ∧ q
---------------------
 T     T         T
 T     F         F
 F     T         F
 F     F         F

```

### The Disjunction Operation (∨)

The proposition **_p_** ∨ **_q_** is read "**_p_** or **_q_**" and is called the **disjunction** of **_p_** and **_q_**.

> **_p_** ∨ **_q_** is TRUE if either **_p_** or **_q_** is true, or if both are true  
> **_p_** ∨ **_q_** is FALSE if both **_p_** and **_q_** are false

```
Truth Table: DISJUNCTION (∨)

 p     q       p ∨ q
---------------------
 T     T         T
 T     F         T
 F     T         T
 F     F         F

```

### The Exclusive Or Operation (⊕)

**inclusive or (∨)** - same as disjunction (∨), TRUE when one or both of the propositions are true<br>
**exclusive or (⊕)** - TRUE when **_p_** is true and **_q_** is false, or when **_p_** is false and **_q_** is true

```
Truth Table: EXCLUSIVE OR (⊕)

 p     q       p ⊕ q
---------------------
 T     T         F
 T     F         T
 F     T         T
 F     F         F

```

### The Negation Operation (¬)

**Negation** - acts on just one proposition by reversing its truth value<br>
The negation of proposition **_p_** is denoted **_¬p_** and is read as "not **_p_**".

```
Truth Table: NEGATION (¬)

 p     ¬p
----------
 T      F
 F      T

```

# 1.2 Evaluating Compound Propositions

Compound propositions may contain more than one logical operator.<br>
The order in which operations are applied in a compound proposition follow the rule:

```
Order of operations without parentheses
applied first → last
---------------------------------------
 ¬ (NOT)    →   ∧ (AND)     →   ∨ (OR)

```

Specifying the order of operations with parentheses:

> **_p_** ∨ **_q_** ∧ **_r_** should be read as **_p_** ∨ (**_q_** ∧ **_r_**)

Because the negation operation is always applied first, the proposition ¬ **_p_** ∨ **_q_** is evaluated as:

> (**_¬p_**) ∨ **_q_** ✅

instead of:

> ¬(**_p_** ∨ **_q_**) ❌

### Filling in the rows of a truth table

A truth table for a compound proposition has a row for every possible combination of truth assignments for the statement's variables.

> If a compound proposition has **_n_** variables, there are 2<sup>n</sup> rows.

The truth table for the compound proposition (**_p_** ∨ **_r_**) ∧ **_¬p_** has 2³ = 8 rows.

# 1.3 Conditional Statements

The **conditional operation** is denoted with the symbol →  
The proposition **_p_** → **_q_** is read "if **_p_**, then **_q_**."

> **_p → q_** is FALSE if **_p_** is true and **_q_** is false; otherwise, **_p → q_** is TRUE

In **_p → q_**, the proposition **_p_** is the **hypothesis**, and the proposition **_q_** is the conclusion.

```
Truth Table: CONDITIONAL (→)

 p     q       p → q
---------------------
 T     T         T
 T     F         F
 F     T         T
 F     F         T

```

_The only way for a conditional statement to be false is if the hypothesis is true and the conclusion is false._  
_If the hypothesis is false, then the conditional statement is true regardless of the truth value of the conclusion._

### English expressions of the conditional operation

Consider the propositions:

> **_p_**: The bears have honey.  
> **_q_**: The bears are happy.

- [If p, then q] // If the bears have honey, then the bears are happy.
- [If p, q] // If the bears have honey, the bears are happy.
- [q if p] // The bears are happy if the bears have honey.
- [p implies q] // Having honey implies that the bears are happy.
- [q whenever p] // The bears are happy whenever they have honey.
- [p only if q] // The bears have honey only if the bears are happy.
- [p is sufficient for q] // The bears having honey is sufficient for them to be happy.
- [q is necessary for p] // The bears being happy is necessary for the bears to have honey.

<br>

### The converse, contrapositive, and inverse

```
Proposition:         p → q    If the bears have honey, the bears are happy.

CONVERSE             q → p    If the bears are happy, the bears have honey.
CONTRAPOSITIVE      ¬q → ¬p   If the bears are not happy, the bears do not have honey.
INVERSE             ¬p → ¬q   If the bears do not have honey, the bears are not happy.

```

<br>

### The biconditional operation

The **biconditional operation** is denoted with the symbol ↔  
The proposition **_p_** ↔ **_q_** is read "**_p_** if and only if **_q_**."

> **_p ↔ q_** is TRUE only when **_p_** and **_q_** have the same truth values

```
Truth Table: BICONDITIONAL (↔)

 p     q       p ↔ q
---------------------
 T     T         T
 T     F         F
 F     T         F
 F     F         T

```
