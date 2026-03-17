# Matlab-MU
Practise and Learning of Matlab programming

The assignment consists of four MATLAB/Octave programs that apply mathematical and computational concepts including matrix operations, arithmetic series, fluid dynamics formulas, and statistical data analysis.   
Each program is menu-driven, input-validated, and structured to demonstrate practical programming skills in a scientific computing environment.\

├──Q1: Random Matrix Generator & Analyser  
├──Q2: Arithmetic Series Calculator  
├──Q3: Air Viscosity Calculator  
├──Q4: Dice Roll Simulator & Histogram Plotter

Random Matrix Generator & Analyser    
[What it does]  
Generates two random matrices of the same user-defined dimensions and performs analysis to find the biggest and smallest elements in each, along with their locations.  
[How it works]  
The program is split into three logical parts:  
1) Input Validation (while loop)  
The user is prompted to enter the number of rows and columns for the matrices. Both must be between 3 and 6 (inclusive). Invalid entries trigger an error message and re-prompt the user until a valid value is supplied.

Matrix Generation
Two matrices, A and B, are generated using randi([0, 100], rows, cols) — filling each matrix with random integers in the range 0 to 100. Both matrices are displayed immediately after generation.

Element Analysis  
The program flattens each matrix using the : operator, finds the maximum and minimum values using max() and min(), then locates each element's row and column position using find(). Results are printed for both matrices.  

Sample Output:    
<img width="645" height="766" alt="image" src="https://github.com/user-attachments/assets/d693045a-fe48-4d9c-9226-00510695017d" />  

<img width="652" height="323" alt="image" src="https://github.com/user-attachments/assets/98aa44f4-72a4-4169-99af-c95959696262" />



[Key MATLAB Concepts Used]  
-while loop with || (OR) operator for input validation  
-randi() for random integer matrix generation  
-max(:) and min(:) with matrix flattening  
-find() for row/column index location

Arithmetic Series Calculator
[What it does]  
A menu-driven arithmetic series calculator that lets the user repeatedly perform calculations on sequences until they choose to exit.

[Formulas Used]  
-Common Difference: d = term2 - term1  
-nth Term: Tn = a + (n-1) * d  
-Sum to n Terms: Sn = (n/2) * (2a + (n-1) * d)  
-where a is the first term and d is the common difference.

[How it works]  
-A while loop keeps the program running as long as the user enters Y or y when asked to continue.   
-A switch statement routes the user's menu selection (1–4) to the appropriate calculation block.   
-Option 4 calls exit() to terminate the program.   
-Invalid options are caught by the otherwise clause.    
<img width="635" height="788" alt="image" src="https://github.com/user-attachments/assets/0863df72-2209-4836-818c-af70e9d05c27" />  

<img width="637" height="369" alt="image" src="https://github.com/user-attachments/assets/ddaf149b-61d0-413a-a2a8-859bc3770baa" />

[Key MATLAB Concepts Used]

-while loop for program repetition  
-switch/case/otherwise for menu routing  
-Arithmetic series formulas implemented as inline expressions  
-input() with string mode for Y/N continuation


Air Viscosity Calculator
[What it does]  
-Calculates the kinematic viscosity of air based on user-supplied temperature and pressure inputs.   
-Uses Sutherland's Law for dynamic viscosity and the ideal gas law for air density.

<img width="368" height="457" alt="image" src="https://github.com/user-attachments/assets/0815fa2c-122e-47e1-aa6a-1d599656217d" />

[How it works]  
-Conversion Stage (runs at start of each loop):  
-The user enters temperature in Celsius, which is converted to Kelvin (T = Tc + 273.15).   
-The user also enters absolute pressure in bars, which is converted to Pascals (P = Pbar × 10⁵).  
-Both converted values are displayed to confirm the conversion.  

Sample Output:
  
<img width="399" height="673" alt="image" src="https://github.com/user-attachments/assets/ca271df4-079d-477b-9665-f2e61ed53fdf" />

<img width="663" height="441" alt="image" src="https://github.com/user-attachments/assets/21bed245-f436-41ac-9d15-2372118a64df" />  

<img width="654" height="551" alt="image" src="https://github.com/user-attachments/assets/f316fe14-9b1d-4a8e-aa17-50e0d2859e2e" />   

<img width="575" height="421" alt="image" src="https://github.com/user-attachments/assets/a9fe68e9-77f2-448f-b4f0-6751c1b189ea" />  

<img width="689" height="547" alt="image" src="https://github.com/user-attachments/assets/2b2ec914-4d44-47c8-8615-9583c00552bd" />

Question 4 — Dice Roll Simulator & Histogram Plotter

[What it does]  
Simulates rolling a 10-sided dice a user-specified number of times, performs statistical analysis on the results, and produces an annotated histogram.

[How it works]  
Part 1 — Dice Roll Simulation:  
-The user enters the number of rolls.   
-The program uses randi([1, 10], 1, rollsNo) to simulate that many rolls of a 10-sided dice, storing results in a row vector.   
-The frequency of each face value (1 through 10) is computed using hist().
  
Part 2 — Statistical Analysis:  
-The program calculates and displays the following statistics from the roll vector  
All six values are stored together in a statistics vector [mean, mode, min, max, stdDev, median].  

Part 3 — Histogram Plot:  
A histogram is plotted with appropriate axis labels and a title. 

<img width="658" height="413" alt="image" src="https://github.com/user-attachments/assets/b50983db-8955-44de-bd43-c069fbe6900e" />  

<img width="685" height="665" alt="image" src="https://github.com/user-attachments/assets/bddb1554-fa3f-4f9a-b7aa-7ad0fc403d32" />  

<img width="577" height="431" alt="image" src="https://github.com/user-attachments/assets/2efe565a-3c6e-4fc5-aa9b-01bf761603be" />  

<img width="721" height="440" alt="image" src="https://github.com/user-attachments/assets/9d0a96de-42b7-4bbc-9294-1f490bbf214d" />  

<img width="591" height="810" alt="image" src="https://github.com/user-attachments/assets/58948212-1dc6-4ae1-ab99-4357d9101ff6" />











