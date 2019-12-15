![College Logo](https://www.gndec.ac.in/logo.png)

# **PROGRAMMING FOR PROGRAM SOLVING ESC-18104/18105**
## **NAME - HARJOT SINGH**
## **ROLL NO - 1921035**
## **SECTION - IT(A2)**

  
# INDEX
1. Program to find Sum
2. Program to print Hello World
3. Program to print a Table
4.  Program to take 5 values from the user and store them in an array and Print the   elements stored in the array
5. Program to use Arithmetic Operators
6. Program to use Assignment Operators
7. Program to use Operator Precedence
8. Program to find Average
9. Program to print Fibbonacci Series
10. Program to find FizzBuzz od a Integer
11. Program swap two numbers using call by value
12. Program swap two numbers using call by reference
13. Program of Addition of 2x2 Matrix
14. Program of Multiplication of 2x2 Matrix
15. Program of FizzBuzz in a continues loop
16. Program to find Sum by using function
17. Program to print a Pyramid
18. Program to implement Linear search for One Dimensional array
19. Program of a Simple Calculator
20. Program to find Factorial


###  1. Program to find Sum

```C
    #include<stdio.h>
    int main()
    {  
         float x,y,z;
    
         printf("\nEnter The First Numder: ");
         scanf("%f", &x);
         printf("\nEnter The Second Numder: ");
         scanf("%f", &y);

         z = x+y;

         printf("\nAnswer is: = %.3f", z);

         return 0;
    }
```  

### Output of the program

    Enter The First Numder: 45.26

    Enter The Second Numder: 78.2648

    Answer is: = 123.525
   
###  2. Program to print Hello World

```C
    #include<stdio.h>
    void main()
    {
         puts("\nHello World\n");
    }
```

### Output of the program

    Hello World

###  3. Program to print a Table

```C
    #include<stdio.h>
    int main()
    {
         float x;
         int n;

         printf("\nEnter The Table: ");
         scanf("%f",&x);

         printf("\nEnter No. Times: ");
         scanf("%d",&n);

         for(int y=1; y<=n; y++)
         {
         printf("\n%.2f x %d = %.3f",x,y,x*y);
         }
         return 0;
    }
```

### Output of the program

    73.00 x 1 = 73.000
    73.00 x 2 = 146.000
    73.00 x 3 = 219.000
    73.00 x 4 = 292.000
    73.00 x 5 = 365.000
    73.00 x 6 = 438.000
    73.00 x 7 = 511.000
    ### 10. Program to take 5 values from the user and store them in an array and Print the elements
### stored in the array

```C
     #include<stdio.h>
     int main()
     {
       int x,array[5];
       printf("\n");
       
       for(x=1;x<=5;x++)
       {  printf("Enter [%d] element: ", x);
          scanf("%d", &array[x]);  }
          
       for(x=1;x<=5;x++)
       {  printf("\nElement [%d] = %d", x, array[x]);  }

     return 0;
     }
```

### Output of the Program

     Enter [1] element: 4
     Enter [2] element: 5
     Enter [3] element: 6
     Enter [4] element: 9
     Enter [5] element: 2

     Element [1] = 4
     Element [2] = 5
     Element [3] = 6
     Element [4] = 9
     Element [5] = 2

###  11. Program to use Arithmetic Operators

```C
    #include<stdio.h>
    int main()
    {
         float x,y,a;

         printf("\nEnter The Value of x: ");
         scanf("%f",&x);

         printf("\nEnter The Value of y: ");
         scanf("%f",&y);

         a = x+y;
         printf("x + y = %.3f\n",a);
         a = x-y;
         printf("x - y = %.3f\n",a);
         a = y-x;
         printf("y - x = %.3f\n",a);
         a = x*y;
         printf("x * y = %.3f\n",a);
         a = x/y;
         printf("x/y = %.3f\n",a);
         a = y/x;
         printf("y/x = %.3f\n",a);

         return 0;
    }
```

### Output of the program

    Enter The Value of x: 45

    Enter The Value of y: 31
    x + y = 76.000
    x - y = 14.000
    y - x = -14.000
    x * y = 1395.000
    x/y = 1.452
    y/x = 0.689

###  12. Program to use Assignment Operators

```C
    #include<stdio.h>
    int main()
    {

         float x,a;

         printf("\nEnter The Value of x: ");
         scanf("%f",&x);

         a = x;
         printf("Answer is a = x %.3f\n",a);
         a +=x; //answer is a+x
         printf("Answer is a+x = %.3f\n",a);
         a -=x; //answer is a-x
         printf("Answer is a-x = %.3f\n",a);
         a *=x; //answer is a*x
         printf("Answer is a*x = %.3f\n",a);
         a /=x; //answer is a/x
         printf("Answer is a/x= %.3f\n",a);

         return 0;
    }
```

### Output of the program

    Enter The Value of x: 45
    Answer is a = x 45.000
    Answer is a+x = 90.000
    Answer is a-x = 45.000
    Answer is a*x = 2025.000
    Answer is a/x= 45.000

###  13. Program to use Operator Precedence

```C
    #include<stdio.h>
 
    int main()
    {
         float a,b,c,d,A;

         printf("\nEnter The Value of a: ");
         scanf("%f",&a);

         printf("Enter The Value of b: ");
         scanf("%f",&b);

         printf("Enter The Value of c: ");
         scanf("%f",&c);

         printf("Enter The Value of d: ");
         scanf("%f",&d);

         A = (a+b)*(c+d);
         printf("\n (a+b)*(c+d) = %.3f",A);
         A = (c+d)*a*b;
         printf("\n (c+d)*a*b = %.3f",A);
         A = a*d/(c-b-a);
         printf("\n a*d/(c-b-a) = %.3f",A);
         A = (b-c)*(a-d);
         printf("\n (b-c)*(a-d) = %.3f",A);

         return 0;
    }
```

### Output of the program

    Enter The Value of a: 45
    Enter The Value of b: 31
    Enter The Value of c: 18
    Enter The Value of d: 71

    (a+b)*(c+d) = 6764.000
    (c+d)*a*b = 124155.000
     a*d/(c-b-a) = -55.086
    (b-c)*(a-d) = -338.000

###  14. Program to find Average

```C
     #include<stdio.h>
     int main()
     {
     int x,N;
     float avg[1000],s,ans;

     printf("\nEnter the Number of elements: ");
     scanf("%d", &N);
     printf("\n");

     for(x=1; x<=N; x++)
       {  printf("Enter [%d] element: ", x);
          scanf("%f", &avg[x]);
          s += avg[x];  }
  
       ans = s/N;

     printf("\nAverage of %d elements = %.3f", N, ans);
     return 0;
     }
```

### Output of the program

     Enter the Number of elements: 8

     Enter [1] element: 1
     Enter [2] element: 2
     Enter [3] element: 3
     Enter [4] element: 4
     Enter [5] element: 5
     Enter [6] element: 6
     Enter [7] element: 7
     Enter [8] element: 8
     
     Average of 8 elements = 4.500    

###  15. Program to print Fibbonacci Series

```C
#include<stdio.h>
int fibbo(int f);

int main()                                                                      
{
   int x,i,f=0;
   printf("\nEnter fibbonacci Number: ");
   scanf("%d", &x);

   for(i=1; i<=x; i++)
     {  printf("%d\n", fibbo(f));
        f++;  }
return 0;
}

int fibbo(int f)
  {  if(f==1 || f==0)
     return f;
     else
     return ( fibbo(f-1) + fibbo(f-2) );  }
```

### Output of the program

    Enter fibbonacci Number: 10
    0
    1
    1 
    2    
    3    
    5    
    8
    13
    21
    34

###  16. Program to find FizzBuzz od a Integer

```C
    #include<stdio.h>
    int main()
    {
         int n;
         printf("\nEnter the Interger: ");
         scanf("%d",&n);

         if(n%15==0)
         printf("\nFizzBuzz");
         else if(n%3==0)
         printf("Fizz\n");
         else if (n%5==0)
         printf("\nBuzz");
         else
         printf("\n%d",n);
         return 0;
    }
```

### Output of the program

    Enter the Interger: 171
    Fizz

###  17. Program swap two numbers using call by value 

```C
    #include <stdio.h>
    int main()
    {
      int x, y, t;
      printf("\n\nEnter two integers: ");
      scanf("%d %d", &x, &y);
      printf("\n\nBefore Swapping: \nFirst integer = %d\nSecond integer = %d\n", x, y);
      t = x;
      x = y;
      y = t;
      printf("\n\nAfter Swapping: \nFirst integer = %d\nSecond integer = %d\n", x, y);
      return 0;
    }
```

### Output of the program

    Enter two integers: 1  56

    Before Swapping:
    First integer = 1
    Second integer = 56

    After Swapping:
    First integer = 56
    Second integer = 1

###  18. Program swap two numbers using call by reference

```C
#include <stdio.h>
void swap(int*, int*);

   int main()
   {  int x, y;
      printf("\nEnter the two integers: ");
      scanf("%d %d", &x, &y);
      printf("\nBefore Swapping\nx = %d\ny = %d", x, y);
      
      swap(&x, &y);
      printf("\nAfter Swapping\nx = %d\ny = %d", x, y);
      return 0;  }
      
   void swap(int *a, int *b)
   {  int temp;
      temp = *b;
      *b = *a;
      *a = temp;  }
```

### Output of the program

     Enter the two integers: 45 98

     Before Swapping
     x = 45
     y = 98
     After Swapping
     x = 98
     y = 45

###  19. Program of Addition of 2x2 Matrix

```C
    #include<stdio.h>
    int main()

    {
         float a,b,c,d,e,f,g,h,i,j,k,l;

         printf("\nSample of Ist matrix: | a=1      b=2 |\n                      | c=3      d=4 |\n\n\
         Sample of 2nd matrix: | e=5      f=6 |\n                      | f=7      h=8 |\n\n");

         printf("Enter The Valve of a: ");
         scanf("%f",&a);
         printf("Enter The Valve of b: ");
         scanf("%f",&b);
         printf("Enter The Valve of c: ");
         scanf("%f",&c);
         printf("Enter The Valve of d: ");
         scanf("%f",&d);
         printf("Enter The Valve of e: ");
         scanf("%f",&e);
         printf("Enter The Valve of f: ");
         scanf("%f",&f);
         printf("Enter The Valve of g: ");
         scanf("%f",&g);
         printf("Enter The Valve of h: ");
         scanf("%f",&h); 
        
         i = a+e;
         j = b+f;
         k = c+g;
         l = d+h;
         printf("\n\nSum of Matrix(A+B) is: | %.2f     %.2f |\n                       | %.2f     %.2f |",i,j,k,l);
        
         i = a-e;
         j = b-f;
         k = c-g;
         l = d-h;
         printf("\n\nSubstraction of Matrix(A-B) is: | %.2f     %.2f |\n                                | %.2f     %.2f |",i,j,k,l);
        
         i = e-a;
         j = f-b;
         k = g-c;
         l = h-d;
         printf("\n\nSubstraction of Matrix(B-A) is: | %.2f     %.2f |\n                                | %.2f     %.2f |",i,j,k,l);
         
         return 0;
    }
```

### Output of the program

    Sample of Ist matrix: | a=1      b=2 |
                          | c=3      d=4 |

    Sample of 2nd matrix: | e=5      f=6 |
                          | f=7      h=8 |

    Enter The Valve of a: 7
    Enter The Valve of b: 5
    Enter The Valve of c: 4
    Enter The Valve of d: 0
    Enter The Valve of e: 3
    Enter The Valve of f: 5
    Enter The Valve of g: 9
    Enter The Valve of h: 1


    Sum of Matrix(A+B) is: | 10.00     10.00 |
                           | 13.00     1.00 |

    Substraction of Matrix(A-B) is: | 4.00     0.00 |
                                    | -5.00     -1.00 |

    Substraction of Matrix(B-A) is: | -4.00     0.00 |
                                    | 5.00     1.00 |

###  20. Program of Multiplication of 2x2 Matrix

```C
    #include<stdio.h>
    int main()
    {
    float a,b,c,d,e,f,g,h,i,j,k,l;

    printf("\nSample of Ist matrix: | a=1      b=2 |\n                      | c=3      d=4 |\n\n\
    Sample of 2nd matrix: | e=5      f=6 |\n                      | f=7      h=8 |\n\n");
 
         printf("Enter The Valve of a: ");
         scanf("%f",&a);
         printf("Enter The Valve of b: ");
         scanf("%f",&b);
         printf("Enter The Valve of c: ");
         scanf("%f",&c);
         printf("Enter The Valve of d: ");
         scanf("%f",&d);
         printf("Enter The Valve of e: ");
         scanf("%f",&e);
         printf("Enter The Valve of f: ");
         scanf("%f",&f);
         printf("Enter The Valve of g: ");
         scanf("%f",&g);
         printf("Enter The Valve of h: ");
         scanf("%f",&h); 

         i=(a*e)+(b*g);
         j=(a*f)+(b*h);
         k=(c*e)+(d*g);
         l=(c*f)+(d*h);

         printf("\nMultiplication of A,B is: | %.2f     %.2f |\n                          | %.2f     %.2f |",i,j,k,l);

         return 0;
    }
```

### Output of the program

    Sample of Ist matrix: | a=1      b=2 |
                          | c=3      d=4 |

    Sample of 2nd matrix: | e=5      f=6 |
                          | f=7      h=8 |

    Enter The Valve of a: 7
    Enter The Valve of b: 5
    Enter The Valve of c: 4
    Enter The Valve of d: 0
    Enter The Valve of e: 3
    Enter The Valve of f: 5
    Enter The Valve of g: 9
    Enter The Valve of h: 1

    Multiplication of A,B is: | 66.00     40.00 |
                              | 12.00     20.00 |

###  21. Program of FizzBuzz in a continues loop

```C
    #include<stdio.h>
    int main()
    {
         int n,x;
         printf("\nEnter The Integer: ");
         scanf("%d",&n);
         printf("\n");

      {
         for(x=1;x<=n;x++)
         if(x%15==0)
         printf("FizzBuzz\n");
         else if(x%3==0)
         printf("Fizz\n");
         else if(x%5==0)
         printf("Buzz\n");
         else
         printf("%d\n",x);
      }

         return 0;
    }
```
### Output of the program

    Enter The Integer: 17

    1
    2
    Fizz
    4
    Buzz
    Fizz
    7
    8
    Fizz
    Buzz
    11
    Fizz
    13
    14
    FizzBuzz
    16
    17
    
### 22. Program to find Sum by using function

```C
      #include<stdio.h>
      int ans(float a, float b);
      int main()
      {
          float a, b, ans;
          printf("\nEnter The Value of a: ");
          scanf("%f",&a);
          printf("Enter The Value of b: ");
          scanf("%f",&b);
          ans = (a*b);
          printf("Answer is: %.2f", ans);
          return 0;
      }
      int ans(float a, float b)
         {
          return a*b;
         }
```         
### Output of the program

      Enter The Value of a: 4
      Enter The Value of b: 5
      Answer is: 20.00
      
### 23. Program to print a Pyramid

```C
     #include<stdio.h>
     int main()
     {
     int i,j,n;
     printf("\nEnter number of Rows: ");
     scanf("%d",&n);
     printf("\n");
     
     for(i=1; i<=n; i++)
     {
         for(j=1; j<=2*n-1; j++)
         {
         if(j>=n-(i-1) && j<=n+(i-1))
         printf("*");
         else
         printf(" ");
         }
         printf("\n");
         }
         return 0;
     }
```

### Output of the program

     Enter number of Rows: 6
     
          *  
         ***    
        *****   
       *******  
      ********* 
     ***********
   
### 24. Program to implement Linear search for One Dimensional array

```C
    #include<stdio.h>
    int main()

    {
    int array[12]={1,5,9,7,3,82,46,23,23,5,10,3};
    int size=12,flag=0,item,a;

    printf("\nEnter the Value: ");
    scanf("%d", &a);

    for(int i=0;i<size;i++)
      {
        if(a==array[i])
          {
                flag=a;
                break;
          }
      }
      
        if(flag==a)
        printf("\nSearch is Sucessfull \n%d Element is present in the array\n",a);
        else
        printf("\nSearch is Unsucessfull \n%d Element is not present in the array\n",a);
        
        return 0;
    }
```
### Output of the program

    First Case

    Enter the Value to be searched: 5

    Search is Sucessfull 5 Element is present in the array
    
    Second Case
    
    Enter the Value to be searched: 2

    Search is Unsucessfull 2 Element is not present in the array
  
  ### 36. Program of a Simple Calculator
    

```C
     include<stdio.h>
     int main()
     {
     char operator;
     float x,y;
     printf("\n\nEnter an operator (+, -, *, /): ");
     scanf("%c", &operator);
     printf("Enter two operands: ");
     scanf("%f %f", &x, &y);
     switch(operator)
     {
             case '+':
             printf("\n%.2f + %.2f = %.2f", x, y, x+y);
             break;
             case '-':
             printf("\n%.2f - %.2f = %.2f", x, y, x-y);
             break;
             case '*':
             printf("\n%.2f * %.2f = %.2f", x, y, x*y);
             break;
             case '/':
             printf("\n%.2f / %.2f = %.2f", x, y, x/y);
             break;
             default:
             printf("\nError! operator is not correct");
     }
     return 0;
     }
```
### Output of the Program

     Enter an operator (+, -, *, /): *
     Enter two operands: 146  21

     146.00 * 21.00 = 3066.00

### 38. Program to find Factorial 

```C
#include<stdio.h>
long factorial(int);

int main()
  {  int x;
     long fact = 1;
     printf("\nEnter a number to calculate it's factorial: ");
     scanf("%d", &x);
     printf("%d! = %ld\n", x, factorial(x));
     return 0;  }

long factorial(int x)
  {  int c;
     long ans=1;
     for (c=x; c>1; c--)
     {  ans *= c;  }
     return ans;
  }
```

### Output of the Program

     Enter a number to calculate it's factorial: 6
     6! = 720

     Enter a number to calculate it's factorial: 12
     12! = 479001600
