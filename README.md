# matrices
import java.util.Scanner;
public class Main
{
    public static void main(String[] args) {
        int a[][]= new int[3][3];
        int b[][]= new int[3][3];
        int c[][]=new int[3][3];
        System.out.println("enter for matrix 1");
        Scanner s = new Scanner(System.in);
        for(int i=0;i<3;i++)
        {
            for(int j=0;j<3;j++)
            {
                    a[i][j]= s.nextInt();
                
            }
        }
        System.out.println();
        System.out.println("enter for matrix 2");
        for(int i=0;i<3;i++)
        {
            for(int j=0;j<3;j++)
            {
                    b[i][j]= s.nextInt();
                
            }
        }
        for(int i=0;i<3;i++)
       {
              for(int j=0;j<3;j++)
            {
                System.out.print(a[i][j]+" ");
            }
            System.out.println("");
        }
     System.out.println();
       
        for(int i=0;i<3;i++)
        {
            for(int j=0;j<3;j++)
            {
                   System.out.print(b[i][j]+" ");
                   
                }
           System.out.println("");
        }
         System.out.println();
        
        System.out.println("on adding two matrices");
       for(int i=0;i<3;i++)
        {
            for(int j=0;j<3;j++)
            {
                   System.out.print((b[i][j]+a[i][j])+" ");
                   
                }
           System.out.println("");
        }
      System.out.println();
        
        System.out.println("on multiplying two matrices");
       for(int i=0;i<3;i++)
        {
            
            for(int j=0;j<3;j++)
            {
                for(int k=0;k<3;k++)
                {
                c[i][j]=c[i][j]+a[i][k]*b[k][i];
                
                }
                System.out.print(c[i][j]+" ");
            }
           System.out.println("");
        }
        
      
    }
}
