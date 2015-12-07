# chinese-remainder-theorem
This project include the endeavour to implement Chinese Remainder Theorem from CS 503
Theorem:
Let n[1],n[2],...,n[k] be positive integers and pairwise coprime. Then the system of simultaneous congruences:
x = a[1](mod n[1])
x = a[2](mod n[2])
.
.
.
x = a[k](mod n[k])
has be UNIQUE solution modulo n = n[1]*n[2]*...*n[k]

Input format:
n[] array and array of a[] in line
Output form:
1) check if the element in n[] is pairwize comprime
2) if it is, output then x

Solution strategy: Gauss Algorithm
Sub-algorithm used in the coding: Extended Euclidean Algorithm

interface format:
1)class CRT(chinese remainder theorem):
input:a)from ASCII file: two lines, in which, first line represent modulos, second line a's, seperated by spaces
      b)from prompt:like a)
      c)int n[], int a[]
output:a)display error message if input don't met requirment
       b)or display the value of the solution
       c)optional: display composition of the x in the form depict below:
         x = (a[1]*(n / n[1])*M[1] + ... + a[k]*(n / n[k])*M[k] ) mod n = final value

2)class EEA(extended euclidean algorithm)
input: int a, int b 
output: int d, int alpha, int beta, as in:
      gcd(a, b) = d
      alpha * a + beta * b = d
