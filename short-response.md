# Problem Set 2.1
## Types, Values, and Operators

1. What is a _unary operator_? Give an example of one.
<br> A _unary operator_ is an operator that takes in one value. An example of a _unary operator_ would be the `typeof` keyword. The `typeof` operator accepts a **single** operand, the operator then returns a string indicating the data type of the operand. 
 
2. What is a _binary operator_? Give an example of one.
<br> A _binary operator_ is an operator which takes in two values. An example of a _binary operator_ could be any multiplicative operator like `*` for example. Multiplicative opertors need two values in order to compare and perform respective tasks.

3. When do we use the _ternary operator_? Use a code snippet to illustrate below.
<br> We use a **ternary operator** when we want to simplify an `if...else` statement. <br>
<br> `condition ? exprIfTrue : exprIfFalse`

4. What is the difference between using the _strict_ and _non-strict_ equality operators?
<br> The **non-strict** equality operator simply compares two values and checks whether or not they are equivalent in value.
The **strict** equality operator checks if two values share the same data type as well as value. 

5. What are the seven JavaScript data types? Which of these are considered _primitive_?
<br> **The seven JavaScript data types include:**
- Strings
- Numbers
- Boolean
- Null
- Undefined
- Symbols
- Objects
<br> **Those of which that are considered _primitive_ include:**
- Strings
- Numbers
- Boolean
- Undefined
- Symbols
- Null
- BigInt

6. What does the code below return?
  ```javascript
  typeof 'i love marcy lab';
  ```
<br> The code would return **String**.

7. What does the code below return?
  ```javascript
  typeof true;
  ```
<br> The code would return **Boolean**. 

8. What does the code below return?
  ```javascript
  typeof (10**9);
  ```
<br>The code would return **Number**. 

9. What does the following code return? **Why**?
  ```javascript
  typeof null;
  ```
<br> The data type `null` represents something that doesn't exist.The output would be object and this is because `null` is used to represent the intentional absence of any object value.

10. What does it mean to be _truthy_ or _falsy_? What six values are _falsy_?
<br> For a value to be _truthy_ it would need to evaluate to true while _falsy_ values are those that evaluate to false. 
<br> **6 values that are _falsy_ are:**
- 0
- (-0)
- " "(empty strings)
- null
- undefined
- NaN  

11. Evaluate the following expressions using JavaScripts implicit coercion rules. For each example, in one sentence, explain what coercions were applied and why:
  * `8 * null` The code snippet features an example of number conversion. Being that the multiplicative operator, `*`, was used; the rule of number conversion calls for both arguments to be converted to numbers and the operator applied respectively. 
  * `true + false` This code snippet displays number conversion. The first rule of number conversion is that `true` converts to 1 and `false` converts to 0. Considering that neither operand is a string, both need to be converted to numbers so the operator can be applied appropriately. 
  * `"i am" + undefined` This code snippet features an example of string conversion. When the binary operator, `+` is applied to operands, if at least one operand is a string, both arguments will be converted to strings and concatenated. 
  * `5 + undefined` This code snippet is an example of number conversion. The rules of number conversion state that `undefined` converts to `NaN` therefore, this snippet would result in `NaN`. 


12. What will each line of the following code return?
   ```javascript
   (false && undefined);
   ```
The following code snippet will return `false`.
   ```javascript
   (false || undefined);
   ```
The following code snippet will return `undefined`.
   ```javascript
   (undefined || false);
   ```
The following snippet will evaluate to `false`. 
   ```javascript
   ((false && undefined) || (false || undefined));
   ```
The following code snippet will evaluate to `undefined`.
   ```javascript
   ((false || undefined) || (false && undefined));
   ```
The following code snippet will return `false`. 
   ```javascript
   ((false && undefined) && (false || undefined));
   ```
The following code snippet will return `false`. 
   ```javascript
   ((false || undefined) && (false && undefined));
   ```
The following code snippet will evaluate to `undefined`.
   ```javascript
   ('a' || (false && undefined) || '');
   ```
The following code snippet will evaluate to `"a"`.
   ```javascript
   ((false && undefined) || 'a' || '');
   ```
The following code snippet will evaluate to `"a"`.
   ```javascript
   ('a' && (false || undefined) && '');
   ```
The following code snippet will evaluate to `undefined`.
   ```javascript
   ((false || undefined) && 'a' && '');
   ```
The following code snippet will evaluate to `undefined`.