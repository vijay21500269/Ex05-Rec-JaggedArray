# Ex05-Rec-JaggedArray
## Aim:
To write a C# program to create a sample CPU usage on a network with 4 nodes using a jagged array.
## Algorithm:
### Step1:
start the program.
### Step2:

Create a jagged array of 4arrays.

int[][] array = new int[4][];

### Step3:
Give the sample CPU usage in the jagged array.


### Step4:
Print the sample CPU usage in the jagged array.


### Step5:
Stop.

## Program:
~~~
using System;
namespace sample
{
    public class cpu_usage
    {
        public static void Main(string[] args)
        {
            int[][] array = new int[4][];
            array[0] = new int[4];
            array[1] = new int[3];
            array[2] = new int[2];
            array[3] = new int[5];
            for(int i=0;i<array.Length;i++)
            {
                for(int j=0;j<array[i].Length;j++)
                {
                    array[i][j] = i * j + 70;
                }
            }
            Console.WriteLine("Total Number of Network Nodes: " + array.Length + "\n");
            for(int i=0;i<array.Length;i++)
            {
                for(int j=1;j<array[i].Length;j++)
                {
                    Console.Write("CPU usage of node in {0} CPU is : {1}%  \n", i, array[i][j]);
                }
            }
        }
    }
}

~~~

## Output:
![EXP5](https://user-images.githubusercontent.com/94381788/230869164-3fc0891d-c61a-4f09-9f23-56cf38f048ff.png)


## Result:
Thus,C# program to create a sample CPU usage on a network with 4 nodes using a jagged array is executed successfully.
