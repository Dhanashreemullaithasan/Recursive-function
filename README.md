# Recursive-function

## Aim: 

To write a C# program to reverse a number using recursive function.

## Algorithm:
## Step 1:

Create a function for reversing.

## Step 2:

Get the number from the user.

## Step 3:

In the function find reminder of the number and multiply it by 10 and add the reverse number.

## Step 4:

Recusively call this function to get the reversed number.

## Step 5:

print the reversed number.

##Program:
```
using System;
namespace Reursive
{
    class Program
    {
        public static int m, rever = 0;
        public static int R(int n)
        {
            if (n>0)
            {
                m = n % 10;
                rever = rever * 10 + m;
                n /= 10;
                return R(n);

            }
            return rever;
        }
        static void Main(string[]args)
        {
            int num;
            Console.WriteLine("Enter a number:");
            num = Convert.ToInt32(Console.ReadLine());
            Console.WriteLine("Reverse of the number:");
            Console.WriteLine(R(num));
        }
    }
}

```
##Output:

![c# ex7](https://github.com/Dhanashreemullaithasan/Recursive-function/assets/94165415/91b76ec0-b169-42ee-98f6-d757a86581c3)

##Result:

Thus the C# program to reverse a number using recursive function is executed successfully.
