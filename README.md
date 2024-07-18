# Quadratic-roots
Quadratic roots program in java
import java.util.Scanner;
public class QuadraticRoots{
    public static void main(String args[]){
        Scanner sc=new Scanner(System.in);
        System.out.println("enter value of a: ");
        double a=sc.nextDouble();
        System.out.println("enter value of b: ");
        double b=sc.nextDouble();
        System.out.println("enter value of c: ");
        double c=sc.nextDouble();
        double discriminant=b*b-(4*a*c);
        if(discriminant>0)
        {
            double root1 = (-b + Math.sqrt(discriminant))/(2*a);
            double root2=(-b - Math.sqrt(discriminant))/(2*a);
            System.out.println("First root is: "+root1+" "+"Second root is: "+root2);
        }
        else if(discriminant==0)
        {
            double root=-b/(2*a);
            System.out.println("Roots are equal and value is: "+root);
        }
        else
        System.out.println("Roots are imaginary");
    }
}
