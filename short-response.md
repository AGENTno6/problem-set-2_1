# Problem Set 2.1
## Types, Values, and Operators

1. What is a _unary operator_? Give an example of one.

A *unary operator* is one that accepts one argument and one argument only. An example of a unary operator would be the `typeOf` operator. 

2. What is a _binary operator_? Give an example of one.

A *binary operator* is an operator that accepts more than one operand. Examples of binary operators include multiplication operator or division operator.

3. When do we use the _ternary operator_? Use a code snippet to illustrate below.

Ternary operators are used to write a more digestible syntax, in other words syntax that is shorter and easier to read. 

`js
if (true) ? console.log("Its litt") : console.log("It's dim");
`
4. What is the difference between using the _strict_ and _non-strict_ equality operators?

The difference between the strict equality operator and the abstract or non-strict equality operator is that one checks for a level of specificity that the other does not. The strict equality operator `===` checks if the operands are of the same data type as well as value while the abstract equality operator checks to see if the two operands are the same in value. The abstract equality operator also converts operands if they are of different data types. 

5. What are the seven JavaScript data types? Which of these are considered _primitive_?

The **7 JavaScript data types** include numbers, booleans, strings, null, undefined, NaN and objects. The data types that constitute as _primitive_ would include **numbers, strings, boolean, null, undefined, NaN and BigInt**. 

6. What does the code below return?
  ```javascript
  typeof 'i love marcy lab';
  ```
<br> **String**

7. What does the code below return?
  ```javascript
  typeof true;
  ```
<br> **Boolean**

8. What does the code below return?
  ```javascript
  typeof (10**9);
  ```
<br> **Number**

9. What does the following code return? **Why**?
  ```javascript
  typeof null;
  ```
<br> **Object**  

10. What does it mean to be _truthy_ or _falsy_? What six values are _falsy_?

<br> When a value is _truthy_ this means that it evaluates to `true`. On the other hand, when a value is _falsy_ that means that it evaluates to `false`. The **6 falsy values** include 0, "", false, `null`, `undefined`, and `NaN`.

11. Evaluate the following expressions using JavaScripts implicit coercion rules. For each example, in one sentence, explain what coercions were applied and why:
  * `8 * null` // `0`
  * `"5" - 1` // `4`
  * `"5" + 1` // `51`
  * `true + false` // `1`
  * `"i am" + undefined` // 'i am undefined'
  * `5 + undefined` // NaN


12. What will each line of the following code return?
   ```javascript
   (false && undefined);
   ```
   <br>**false** 

   ```javascript
   (false || undefined);
   ```
   <br> **false**
   
   ```javascript
   (undefined || false);
   ```
   <br> **false**

   ```javascript
   ((false && undefined) || (false || undefined));
   ```
   <br> **undefined**

   ```javascript
   ((false || undefined) || (false && undefined));
   ```
   <br> **Undefined**

   ```javascript
   ((false && undefined) && (false || undefined));
   ```
    <br> **False** BUT WHY??


   ```javascript
   ((false || undefined) && (false && undefined));
   ```

   ```javascript
   ('a' || (false && undefined) || '');
   ```

   ```javascript
   ((false && undefined) || 'a' || '');
   ```

   ```javascript
   ('a' && (false || undefined) && '');
   ```

   ```javascript
   ((false || undefined) && 'a' && '');
   ```
