# Heading-Averager---SRM-AUV
Program to find Heading Averager
#include<iostream.h>
#include<conio.h>
/*This program will continue to input values from AUV compass within 0 to 360 range
To find output the average,users need to input
This program will work for infinite number of inputs*/

void main()
{
  clrscr();
  float reading,avg,sum=0,count=0;
  do
  {
     cout<<"Enter Reading ";
     cin>>reading;
     if(reading == -1)
       break;
     ++count;
     sum+= reading;
     avg = sum / count;
  }while(reading>=0 && reading<=360);
  cout<<"The heading Averager is "<<avg;
  getch();
}

