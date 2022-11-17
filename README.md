FACTORIAL 

#! bin/bash 

echo "Welcome to Factorial Calculation"
echo "Enter a Number:"
read n
fact=1
for ((i=1;i<n+1;i++))
do
fact=$((fact*i))
done
echo "Factorial of "$n "is:" $fact

SUM OF N NUMBERS

 #! bin/bash
echo "Welcome to Sum of N number Calculation"
echo "Enter the limit:"
read a
sum=0
for ((i=0;i<=a;i++))
do
sum=$((sum+i))
done
echo "Sum upto" $a "Numbers is:"$sum

FIBONACCI SERIES 

#! /bin/bash
echo "Welcome to Fibbonaci Series"
echo "Enter the limit:"
read n
a=0
b=1
for ((i=0;i<n;i++))
do
echo -n " $a"
fibbo=$((a+b))
a=$b
b=$fibbo
done

ALU

#!/bin/bash

echo "Welcome to ALU "
echo "Enter number1 : "
read a
echo "Enter number2 : "
read b
echo "Enter operation to perform : "
read n
if [ $n == 1 ]
then
ans=expr $a + $b
echo "Sum is : $ans"
elif [ $n == 2 ]
then
ans=expr $a - $b
echo "Difference is : $ans"
elif [ $n == 3 ]
then
ans=expr $a \* $b
echo "Multiplication is : $ans"
elif [ $n == 4 ]
then
ans=expr $a / $b
echo "Division is : $ans"
fi

GREATEST OF 3NUMBERS 

#!/bin/bash
echo "Enter the first number:"
read a
echo "Enter the second number:"
read b
echo "Enter the third number:"
read c
if [ $a -gt $b ] && [ $a -gt $c ]
then
echo "The Greater Number is:" $a
elif [ $b -gt $a ] && [ $b -gt $c ]
then
echo "The Greater Number is:" $b
else
echo "The Greater Number is:" $c

fi
