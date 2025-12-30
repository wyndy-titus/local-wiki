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

# 1.4 Logical Equivalence

**tautology** - a compound proposition that is always true regardless of the truth value of its individual propositions  
**contradiction** - a compound proposition that is always false regardless of the truth value of its individual propositions

> **_p_** ∨ **_¬p_** is a tautology since the proposition is always true whether **_p_** is true or false  
> **_p_** ∧ **_¬p_** is a contradiction since the proposition is always false regardless of whether **_p_** is true or false

```
Truth Table: TAUTOLOGY (p ∨ ¬p)

 p     ¬p      p ∨ ¬p
---------------------
 T      F        T
 F      T        T

```

```
Truth Table: CONTRADICTION (p ∧ ¬p)

 p     ¬p      p ∧ ¬p
---------------------
 T      F        F
 F      T        F

```

<br>

Two compound propositions are **logically equivalent** if they have the same truth value regardless of the truth values of their individual propositions.

> If **_s_** and **_r_** are two compound propositions, the notation **_s_** ≡ **_r_** is used to indicate that **_s_** and **_r_** are logically equivalent.

Propositions **_s_** and **_r_** are logically equivalent if and only if the proposition **_s_** ↔ **_r_** is a tautology.

### De Morgan's Laws

**De Morgan's laws** are logical equivalences that show how to correctly distribute a negation operation inside a parenthesized expression.

> ¬(**_p_** ∨ **_q_**) ≡ (**_¬p_** ∧ **_¬q_**)

When the negation operation is distributed inside the parenthesis, **the disjunction operation changes to a conjunction operation.**

Given the following propositions:

> **_p_**: The patient has migraines.  
> **_q_**: The patient has high blood pressure.

De Morgan's law says that the following two statements are logically equivalent:

> It is not true that the patient has migraines or high blood pressure.  
> The patient does not have migraines and does not have high blood pressure.

```
Truth Table to show: ¬(p ∨ q) ≡ (¬p ∧ ¬q)

 p    q    ¬p    ¬q     p ∨ q     ¬(p ∨ q)     ¬p ∧ ¬q
-------------------------------------------------------
 T    T     F     F       T           F           F
 T    F     F     T       T           F           F
 F    T     T     F       T           F           F
 F    F     T     T       F           T           T

```

The second version of De Morgan's law swaps the role of the disjunction and conjunction:

> ¬(**_p_** ∧ **_q_**) ≡ (**_¬p_** ∨ **_¬q_**)

Continuing with the same example, the following two statements are logically equivalent:

> It is not true that the patient has migraines and high blood pressure.  
> The patient does not have migraines or does not have high blood pressure.

```
Truth Table to show: ¬(p ∧ q) ≡ (¬p ∨ ¬q)

 p    q    ¬p    ¬q     p ∧ q     ¬(p ∧ q)     ¬p ∨ ¬q
-------------------------------------------------------
 T    T     F     F       T           F           F
 T    F     F     T       F           T           T
 F    T     T     F       F           T           T
 F    F     T     T       F           T           T

```

### Examples for logically equivalent statements:

1️⃣ It is not true that an average person sleeps more than 8 hours or commutes to work less than 30 minutes each day.

STEP 1 - Find **_p_** and **_q_**

> **_p_**: An average person sleeps more than 8 hours.  
> **_q_**: An average person commutes to work less than 30 minutes each day.

STEP 2 - Translate the statement into its logical proposition

> It is **not true** that an average person sleeps more than 8 hours **or** commutes to work less than 30 mins each day.  
> That statement is equivalent to **¬(p ∨ q)**.

STEP 3 - Use De Morgan's law to find the equivalent statement

> Since the original statement is **¬(p ∨ q)**, by De Morgan's law, its equivalent statement is (**_¬p_** ∧ **_¬q_**).

STEP 4 - Translate the logical proposition to its equivalent statement

> (**_¬p_** ∧ **_¬q_**)  
> **_¬p_** -> An average person **does not** sleep more than 8 hours. // (**at most** 8 hours)  
> **_¬q_** -> An average person **does not** commute to work less than 30 mins each day. // (**at least** 30 mins)

<br>

2️⃣ It is not true that the pizza has at least 3 types of cheese and at most 4 toppings.

STEP 1 - Find **_p_** and **_q_**

> **_p_**: The pizza has at least 3 types of cheese.  
> **_q_**: The pizza at most has 4 toppings.

STEP 2 - Translate the statement into its logical proposition

> It is **not true** that the pizza has at least 3 types of cheese **and** at most 4 toppings.  
> That statement is equivalent to **¬(p ∧ q)**.

STEP 3 - Use De Morgan's law to find the equivalent statement

> Since the original statement is **¬(p ∧ q)**, by De Morgan's law, its equivalent statement is (**_¬p_** ∨ **_¬q_**).

STEP 4 - Translate the logical proposition to its equivalent statement

> (**_¬p_** ∨ **_¬q_**)
> **_¬p_** -> The pizza **does not** have at least 3 types of cheese. // (**has less than** 3 types of cheese)  
> **_¬q_** -> The pizza **does not** have at most 4 toppings. // (**has more than** 4 toppings)

<br>

# 1.5 Laws of Propositional Logic

<br>

<table>
    <tr>
        <th>Law</th>
        <th>Version 1</th>
        <th>Version 2</th>
    </tr>
    <tr>
        <td>Idempotent</td>
        <td>p ∨ p ≡ p</td>
        <td>p ∧ p ≡ p</td>
    </tr>
    <tr>
        <td>Associative</td>
        <td>(p ∨ q) ∨ r ≡ p ∨ (q ∨ r)</td>
        <td>(p ∧ q) ∧ r ≡ p ∧ (q ∧ r)</td>
    </tr>
    <tr>
        <td>Commutative</td>
        <td>p ∨ q ≡ q ∨ p</td>
        <td>p ∧ q ≡ q ∧ p</td>
    </tr>
    <tr>
        <td>Distributive</td>
        <td>p ∨ (q ∧ r) ≡ (p ∨ q) ∧ (p ∨ r)</td>
        <td>p ∧ (q ∨ r) ≡ (p ∧ q) ∨ (p ∧ r)</td>
    </tr>
    <tr>
        <td>Identity</td>
        <td>p ∨ F ≡ p</td>
        <td>p ∧ T ≡ p</td>
    </tr>
    <tr>
        <td>Domination</td>
        <td>p ∧ F ≡ F</td>
        <td>p ∨ T ≡ T</td>
    </tr>
    <tr>
        <td>Double negation</td>
        <td>¬¬p ≡ p</td>
        <td>&nbsp;</td>
    </tr>
    <tr>
        <td>Complement</td>
        <td>p ∧ ¬p ≡ F <br> ¬T ≡ F</td>
        <td>p ∨ ¬p ≡ T <br> ¬F ≡ T</td>
    </tr>
    <tr>
        <td>De Morgan's</td>
        <td>¬(p ∨ q) ≡ ¬p ∧ ¬q</td>
        <td>¬(p ∧ q) ≡ ¬p ∨ ¬q</td>
    </tr>
    <tr>
        <td>Absorption</td>
        <td>p ∨ (p ∧ q) ≡ p</td>
        <td>p ∧ (p ∨ q) ≡ p</td>
    </tr>
    <tr>
        <td>Conditional identity</td>
        <td>p → q ≡ ¬p ∨ q</td>
        <td>p ↔ q ≡ (p → q) ∧ (q → p)</td>
    </tr>
</table>

<!--
| Law             |            Version 1            |            Version 2            |
| --------------- | :-----------------------------: | :-----------------------------: |
| Idempotent      |            p ∨ p ≡ p            |            p ∧ p ≡ p            |
| Associative     |    (p ∨ q) ∨ r ≡ p ∨ (q ∨ r)    |    (p ∧ q) ∧ r ≡ p ∧ (q ∧ r)    |
| Commutative     |          p ∨ q ≡ q ∨ p          |          p ∧ q ≡ q ∧ p          |
| Distributive    | p ∨ (q ∧ r) ≡ (p ∨ q) ∧ (p ∨ r) | p ∧ (q ∨ r) ≡ (p ∧ q) ∨ (p ∧ r) |
| Identity        |            p ∨ F ≡ p            |            p ∧ T ≡ p            |
| Domination      |            p ∧ F ≡ F            |            p ∨ T ≡ T            |
| Double negation |             ¬¬p ≡ p             |                                 |
| Complement      |     p ∧ ¬p ≡ F <br> ¬T ≡ F      |     p ∨ ¬p ≡ T <br> ¬F ≡ T      |
| De Morgan's     |       ¬(p ∨ q) ≡ ¬p ∧ ¬q        |       ¬(p ∧ q) ≡ ¬p ∨ ¬q        |
| Absorption      |         p ∨ (p ∧ q) ≡ p         |         p ∧ (p ∨ q) ≡ p         |
| Conditional     |         p → q ≡ ¬p ∨ q          |    p ↔ q ≡ (p → q) ∧ (q → p)    |
-->
<br>

### Using the laws of propositional logic to show logical equivalence

Completing the proof: **¬(p → q) ≡ p ∧ ¬q**

STEP 1 - Start with the expression on the left of the equivalence

> ¬(p → q)

STEP 2 - Apply the conditional identity [a → b ≡ ¬a ∨ b]

> ¬(¬p ∨ q)

STEP 3 - Apply De Morgan's law [¬(a ∨ b) ≡ ¬a ∧ ¬b]

> ¬¬p ∧ ¬q

STEP 4 - Apply the double negation law [¬¬a ≡ a]

> p ∧ ¬q
