java c1. You will use object-oriented techniques, file processing, data types and structures you have learned throughout the semester to solve problems.
2. Submission requirements:
a. You should only submit one zip-folder with your Java project code. Only English solutions and comments are accepted. Answers need to be zipped as a java project. 
b. Please name your Java project code in ONE zip folder as ‘Coursework3_YourID.’ 
c. You also need to submit a report in PDF format that explains the task, how you understood the question, and why you believe your solution is the best approach.
Matrix Operations
This year, you are required to complete a class that implements matrix operations. The tasks involve creating a Matrix class with various methods to handle operations such as addition, subtraction, multiplication, transposition, and determinant calculation. Please download the provided code template from the Learning Mall before starting the assignment. The template will give you a structured starting point for your implementation. Once you have completed writing your code, paste the code for each method into the respective submission boxes on the Learning Mall. The following is a detailed description of the task.
 
Important Note: Pay close attention to edge cases and ensure that your methods handle invalid inputs gracefully. Failure to do so will result in significant point deductions.
 
 
Task 1: Matrix Class Implementation (10 marks)
Implement the constructor for the class Matrix that will handle basic matrix operations.
● A constructor public Matrix(double[][] data) to initialize the matrix. If the input data is null or not a proper 2D array (rows with different lengths), throw an IllegalArgumentException.
 
 
Task 2: Accessor Method (10 marks)
Implement a method to retrieve the matrix data:
● public double[][] getData(): This method should return a deep copy of the data field to prevent external modification.
 
 
Task 3: Matrix Addition (15 marks)
Implement a method to add two matrices:
● public Matrix add(Matrix other): This method should add the corresponding elements of the matrices and return a new Matrix object with the result. If the matrices are not of the same size, throw an IllegalArgumentException.
 
 
Task 4: Matrix Subtraction (15 marks)
Implement a method to subtract another matrix from the current matrix:
● public Matrix subtract(Matrix other): This method should subtract the corresponding elements of the other matrix from the current matrix and return a new Matrix object with the result. If the matrices are not of the same size, throw an IllegalArgumentException.
 
 
Task 5: Matrix Multiplication (20 marks)
Implement a method to multiply the current matrix with another matrix:
● public Matrix multiply(Matrix other): This method should perform matrix multiplication and return a new Matrix object with the result. If the number of columns in the current matrix does not match the number of rows in the other matrix, throw an IllegalArgumentException.
 
 
Task 6: Matrix Transposition (10 marks)
Implement a method to transpose the current matrix:
● public Matrix transpose(): This method should return a new Matrix object with the transposed matrix.
 
 
Task 7: Matrix Determinant (20 marks)
Implement a method to calculate the determinant of the matrix:
● public double determinant(): This method should return the determinant of the matrix. For non-square matrices, throw an IllegalArgumentException. Implement determinant calculation for 2x2 and 3x3 matrices. For matrices larger than 3x3, return Double.NaN.
 
Example Usage and Output
This section does not need to be submitted.
 
public static void main(String[] args) {
   double[][] data1 = {{1, 2}, {3, 4}};
   double[][] data2 = {{5, 6}, {7, 8}};
   
   Matrix matrix1 = new Matrix(data1);
   Matrix matrix2 = new Matrix(data2);
   
   Matrix sum = matrix1.add(matrix2);
   Matrix difference = matrix1.subtract(matrix2);
   Matrix product = matrix1.multiply(matrix2);
   Matrix transpose = matrix1.transpose();
   double determinant = matrix1.determinant();
   
   // Print results
   System.out.println("Sum:");
   printMatrix(sum.getData());
   System.out.println("Difference:");
   printMatrix(difference.getData());
   System.out.println("Product:");
   printMatrix(product.getData());
   System.out.println("Transpose:");
   printMatrix(transpose.getData());
   System.out.println("Determinant:");
   System.out.println(determinant);
}
 
private static void printMatrix(double[][] matrix) {
   for (double[] ro代 写program 、 Python /Java
代做程序编程语言w : matrix) {
       for (double val : row) {
           System.out.print(val + " ");
       }
       System.out.println();
   }
}
 
The output should be:
Sum:
6.0 8.0 
10.0 12.0 
Difference:
-4.0 -4.0 
-4.0 -4.0 
Product:
19.0 22.0 
43.0 50.0 
Transpose:
1.0 3.0 
2.0 4.0 
Determinant:
-2.0
Report 
In this report, you should document your understanding of the task and provide a justification for your solution. You should also explain why you believe your code structure is well-designed and clear. Additionally, you need to test edge cases and provide a technically sound report on how your code handles these cases.. 
 
The marking is distrubuted as follows:
 
● Understanding of the Task: 30 marks
● Justification of Solution: 30 marks
● Clarity and Structure: 20 marks
● Handling of Edge Cases: 10 marks
● Technical Accuracy: 10 marks
 
Below is the marking details of report:
Criteria	Excellent (90-100 marks)	Good (75-89 marks)	Satisfactory (60-74 marks)	Needs Improvement (40-59 marks)	Poor (0-39 marks)
Understanding of the Task (30 marks)	Demonstrates a deep and comprehensive understanding of the task; accurately identifies all key requirements and constraints.	Demonstrates a good understanding of the task; identifies most key requirements and constraints.	Demonstrates a basic understanding of the task; identifies some key requirements and constraints, but with minor misunderstandings or omissions.	Demonstrates a limited understanding of the task; identifies few key requirements and constraints with significant misunderstandings or omissions.	Shows little to no understanding of the task; fails to identify key requirements and constraints.
Justification of Solution (30 marks)	Provides a well-reasoned and convincing argument for why the solution is optimal, considering multiple factors such as efficiency, scalability, and edge case handling.	Provides a solid argument for the solution, considering important factors like efficiency and scalability, though some reasoning may be less developed.	Provides a basic argument for the solution, with some consideration of factors like efficiency, but lacks depth or fails to address key aspects.	Provides a weak or unconvincing argument for the solution, with little consideration of important factors or only superficial reasoning.	Provides no clear justification for the solution, or the justification is irrelevant or flawed.
Clarity and Structure (20 marks)	Report is well-organized, with clear, logical progression; explanations are concise, precise, and easy to follow.	Report is well-organized, with minor lapses in clarity or structure; explanations are generally clear, but may occasionally be wordy or unclear.	Report is somewhat organized but may have several unclear sections or lack of logical flow; explanations are adequate but may be verbose or confusing.	Report is poorly organized, with significant lapses in clarity or structure; explanations are often unclear or confusing.	Report is disorganized, with little to no clear structure; explanations are unclear, incomplete, or difficult to follow.
Handling of Edge Cases (10 marks)	Thoroughly addresses all potential edge cases, with clear and correct reasoning for how they are handled in the code.	Addresses most edge cases, with generally correct reasoning for how they are handled, though some cases may be overlooked or inadequately explained.	Addresses some edge cases, but may overlook important ones or provide insufficient explanations for how they are handled in the code.	Addresses few edge cases, with minimal or flawed reasoning for how they are handled in the code.	Fails to address edge cases or provides incorrect or incomplete explanations.
Technical Accuracy (10 marks)	The technical explanation is accurate and demonstrates a strong understanding of matrix operations, including correct terminology and implementation details.	The technical explanation is mostly accurate, with minor errors or omissions; demonstrates a good understanding of matrix operations, though some details may be slightly off.	The technical explanation has some inaccuracies or misunderstandings; demonstrates a basic understanding of matrix operations, but may misuse terminology or overlook important details.	The technical explanation has significant inaccuracies or misunderstandings; demonstrates limited understanding of matrix operations and often misuses terminology or omits important details.	The technical explanation is largely inaccurate, with frequent misunderstandings and misuse of terminology; shows little to no understanding of matrix operations.

         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
