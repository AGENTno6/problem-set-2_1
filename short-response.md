# Problem Set 2.1
## Types, Values, and Operators

1. What is a _unary operator_? Give an example of one.

 A **Unary operator** is an operator that takes in one value.
 An example of a unary operator would be the `typeOf` keyword.
 
2. What is a _binary operator_? Give an example of one.
A **binary operator** is an operator which takes in two values. An example of a binary operator could be any multiplicative operator like `*`. These multiplicative opertors need two values in order to compare and perform respective tasks.

3. When do we use the _ternary operator_? Use a code snippet to illustrate below.
We use a **ternary operator** when we want to simplify an `if...else` statement.

`condition ? exprIfTrue : exprIfFalse`

4. What is the difference between using the _strict_ and _non-strict_ equality operators?
The **non-strict** equality operator simply compares two values and checks whether or not they are the same.
The **strict** equality operator checks if two values share the same data type as well as if they're equal in value. 

5. What are the seven JavaScript data types? Which of these are considered _primitive_?
The seven JavaScript data types include:
-Strings
-Numbers
-Boolean
-Null
-Undefined
-Symbols
-Objects

Those of which that are considered _primitive_ include:
-Strings
-Numbers
-Boolean
-Undefined
-Symbols
-Null
-Bigint

6. What does the code below return?
  ```javascript
  typeof 'i love marcy lab';
  ```
**String**

7. What does the code below return?
  ```javascript
  typeof true;
  ```
**Boolean**

8. What does the code below return?
  ```javascript
  typeof (10**9);
  ```
**Number**

9. What does the following code return? **Why**?
  ```javascript
  typeof null;
  ```
The data type `null` represents something that doesn't exist.The output would be object and this is because `null` is often used to signify an empty reference to an object.

10. What does it mean to be _truthy_ or _falsy_? What six values are _falsy_?

For a value to be _truthy_ it would need to evaluate to true.
_Falsy_ values are those that evaluate to false. 
6 values that are _falsy_ are:
-0
-(-0)
-" "(empty strings)
-null
-undefined
-NaN  

11. Evaluate the following expressions using JavaScripts implicit coercion rules. For each example, in one sentence, explain what coercions were applied and why:
  * `8 * null`
  * `"5" - 1`
  * `"5" + 1`
  * `true + false`
  * `"i am" + undefined`
  * `5 + undefined`


12. What will each line of the following code return?
   ```javascript
   (false && undefined);
   ```

   ```javascript
   (false || undefined);
   ```
   
   ```javascript
   (undefined || false);
   ```

   ```javascript
   ((false && undefined) || (false || undefined));
   ```

   ```javascript
   ((false || undefined) || (false && undefined));
   ```

   ```javascript
   ((false && undefined) && (false || undefined));
   ```

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
