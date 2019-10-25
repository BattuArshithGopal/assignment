import java.util.*;
class Main
{
public static void main(String[]args)
{
Scanner in = new Scanner(system.in)
Scanner in = new Scanner(System.in);
      System.out.println("Enter number of units used:");
      float n = in.nextFloat();
      float cu,c;
      float ed = 0.06;
      float r1,r2,r3,r4,r5;
      System.out.println("Enter the five slab rates:");
       r1 = in.nextInt();
       r2 = in.nextInt();
       r3 = in.nextInt();
       r4 = in.nextInt();
       r5 = in.nextInt();
      if(n<=100)
      {
        cu = 100;
      }
      else if(n<=101&&n<=200)
      {
        cu = 40;
      }
      else
      {
        cu = 55;
      }
      if(n<=50)
      {
        c=n*r1+cu+ed*n;
      }
      else if(n<=51&&n<=100)
      {
        c=50*r1+(n-50)*r2+cu+ed*n;
      }
      else if(n<=101&&n<=200)
      {
        c=50*r1+50*r2+(n-100)*r3+cu+ed*n;
      }
      else if(n<=201&&n<=300)
      {
        c=50*r1+50*r2+100*r3+(n-200)*r4+cu+ed*n;
      }
      else
      {
        c=50*r1+50*r2+100*r3+100*r4+(n-300)*r5+cu+ed*n;
      }
      System.out.println("Electricity bill is :" +c);
      }
      }
