# ARTI 303 — Lab 04, Task 2

## Queries and answers

1. **Show the names of all females**
   ```prolog
   ?- female(X).
   ```
   **Answer:** `X = sara; X = nora.`

2. **Check whether there is any male**
   ```prolog
   ?- male(_).
   ```
   **Answer:** `true.`

3. **Show the grandparent of Faisal**
   ```prolog
   ?- parent(X, Y), parent(Y, faisal).
   ```
   **Answer:** `X = ali, Y = muhammad.`

4. **Show all daughters of Ahmad**
   ```prolog
   ?- parent(ahmad, X), female(X).
   ```
   **Answer:** `X = sara; X = nora.`

5. **Check whether Ahmad and Muhammad have a common parent**
   ```prolog
   ?- parent(P, ahmad), parent(P, muhammad).
   ```
   **Answer:** `P = ali.` Yes, they have a common parent.

6. **Check whether Khan is the brother of Nora**
   ```prolog
   ?- male(khan), parent(P, khan), parent(P, nora).
   ```
   **Answer:** `P = ahmad.` Yes, Khan is Nora's brother.
