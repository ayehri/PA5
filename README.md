# PA5 - Introduction to MATLAB Programming

## Intended Learning Outcomes
1. To identify the codes and built-in functions used in MATLAB Programming.
2. To be able to apply and use the different codes and built-in functions in creating a MATLAB
program.

# Problem 1
<img width="597" height="118" alt="image" src="https://github.com/user-attachments/assets/3d18dfc4-2099-4d8f-8bf0-db88b6ec10f2" />

### Code:
<img width="653" height="455" alt="image" src="https://github.com/user-attachments/assets/4acef9c2-a074-4ed3-9f8b-232648e21023" />

### Output:
<img width="557" height="428" alt="image" src="https://github.com/user-attachments/assets/6838cf65-675e-480c-b79f-213c9e2cb99c" />
<img width="588" height="300" alt="image" src="https://github.com/user-attachments/assets/9715f5b1-0b46-4dfd-961d-e36ec078aea3" />

### Explanation:
Matrix A (Real Matrix)
- x: matrix with real numbers
- y = x': Conjugate transpose operation. y is switched with x
- z = x.': Transpose operation which will flip the rows and columns
  
Matrix B (Complex Matrix)
- i: Matrix with complex numbers
- j = i': Conjugate transpose operation. Flips the matrix and changes the sign of the imaginary numbers.
- k = i.': Transpose operation. Flips the matrix but does not change the signs of the imaginary numbers.
- They will both produce different results since the matrix is complex unlike in Matrix A.

# Problem 2
<img width="604" height="164" alt="image" src="https://github.com/user-attachments/assets/1086ee2c-8740-4852-b6e4-9427ce118dce" />

### Code:
<img width="386" height="457" alt="image" src="https://github.com/user-attachments/assets/d32b9dc1-b25d-4216-a550-1cf62ebdf9c9" />

### Output:
<img width="120" height="406" alt="image" src="https://github.com/user-attachments/assets/2bdafddf-f986-41cc-9cbc-2eef9d8a6735" />

### Explanation: 
- x: The coefficients of the varaiable in each equation.
- y: The constants on the right side of the equation.
- z = inv(x)*y: This expression can be used to solve the inverse of the matrix x and y.
- disp(z): Displays the inverse vector
- n = size(x,1): gets the number of variables.
- e = zeros(n,1): Creates space to store each variable's solution.
- d = x;: Copy of the original coefficient matrix.
- d(:,c) = y;: replaces the column c with constants.
- e(c) = det(d)/det(x);: Cramer's rule formula to solve for the variable.
- end: To close or stop the for loop.
- disp(e):  Displays the final solution vector

# Conclusion:
For Problem 1, we learned the difference between the transpose (.') and the conjugate transpose (') operations in MATLAB. When the matrix contains only real numbers, both operations give the same result because there are no imaginary parts to change. However, in the complex matrix, the conjugate transpose changes the signs of the imaginary components, while the transpose only changes the positions of the elements. This shows that the two operations produce the same output only for real matrices, but not for complex matrices.

For Problem 2, we solved a system of linear equations using both the Inverse Method and Cramer's Rule. Both methods produced the same solution vector, which confirms that the calculations are accurate and that both methods are valid for solving systems of linear equations.
