# Anand.java
public class Guru {
    public static void main(String args [])
    {
        int  matrix[][]  = {{1,2,3,} ,{4,5,6,},{7,8,9}};
        for(int row = 0; row<3;row++)
        {
            if((row + 2) % 2==0)
            {
                for(int col = 0 ;col<3;col++)
                {
                    System.out.print(matrix[row][col]+" ");
                }
            }
            else
                for(int col =2 ;col>=0; col--)
                {
                    System.out.print(matrix[row][col]+" ");
                }
    }
}}
class Anna extends Guru{
    public static void main( String args[])
    {
        int mat[][]= {{6,5,4,},{1,2,5,},{7,9,7,}};
        int s=0;
        int sum =0;

        for (int row = 0; row < 3;row++)
        {
            for (int col =row ;col<3;col++)
            {
                System.out.print(mat[row][col]+" ");
                s+=mat[row][col];
            }
            System.out.println();
        }
        System.out.println(s);
        for (int row = 0;row <3;row++)
        {
            for (int col = 0; col <= row ;col++)
            {
                System.out.print(mat[row][col]+" ");
                sum = sum + mat[row][col];
            }
            System.out.println();
        }
        System.out.print(sum);

    }
}
