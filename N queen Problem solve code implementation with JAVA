/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */
package javaapplication1;


/**
 *
 * @author ADG
 */
public class JavaApplication1 {

  
    public static void main(String[] args) {
        //int arr[][]={{6,1,10,2},{7,11,4,14},{5,890,9,15},{8,12,13,3}};  
        //int arr1[] = {6,1,10,2,7,11,4,14,5,890,9,15,8,12,13,3};
        int arr[][] = {{7,1,2},{5,66,4},{8,3,6}};
        int arr1[]= {7,1,2,5,66,4,8,3,6};
        
        int sum[] ={};
        int calc = 0,k = 0,inv =0;
        for(int i=0;i<8;i++)
        {
            System.out.print(arr1[i] + " ---> " );
            for(int j=i;j<8;j++)
            {
                
                if (arr1[i]>arr1[j+1] && arr1[i] != 66) // checks if the number is bigger and whether its blank tile
                {
                    calc++; // calc increases as by the condition satisfies
                    //System.out.println(arr1[i] +" less than " + arr1[j+1]);
                }
                
                System.out.print( arr1[j+1] + " ");
                
            }
            System.out.println(calc);
            inv = inv+ calc; // for every tile the sum is added to the inversion  number
            calc=0; // calc is reset to zero
           
        }
        System.out.println(inv);
        
        int row=0;
        int col=0;
        for(int i=0;i<arr.length;i++)
        {
            for(int j=0;j<arr.length;j++)
            {
                if (arr[i][j] == 66)
                {
                    System.out.println((i) + " th row " + (j) + " th column");
                    row=i;
                    col=j;
                }
            }
        }
        
        
         int dim = arr.length+1;
    
         boolean Check = oddevenCount(dim);
         
         if((Check == false) && (oddevenCount(inv) == false))
                 {
                     System.out.println("Solveable");
                 }
         else if((Check == true) && (oddevenCount(inv) == true) && (oddevenCount(row)==false ))
                 {
                     System.out.println("Solveable");
                 }
         else if((Check == true) && (oddevenCount(inv) == false) && (oddevenCount(row)==true ))
                 {
                     System.out.println("Solveable");
                 }
         else
         {
             System.out.println("Not solveable");
         }
    }
    
    public static boolean oddevenCount(int a)
    {
        boolean xy;
        if ((a % 2) == 0)
            {
                xy = true;
            }
            else
                {
                    xy = false;
                }
        return xy;
    }
    
   
    
    
}
