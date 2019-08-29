package javaapplication24;

import java.util.Scanner;

/**
 *
 * @author LENOVO
 */
public class JavaApplication24 {

    /**
     * @param args the command line arguments
     */
         public static void main(String[] args) {
          Scanner sc = new Scanner(System.in);
         
        int i;
        System.out.println("Input size of array: ");
        int kol=sc.nextInt();
        int[]array=new int[kol];
        boolean sym = true;
       
        System.out.println("Input elements of array: ");
        for( i=0; i<kol; i++)
           array[i]=sc.nextInt();
        
      
      
    System.out.println("Result");
        for( i=0; i<kol; i++)
            System.out.print(array[i]+" ");

          for(i=0;i<kol/2;i++){
        if(array[i]!= array[kol-1-i]){
        sym=false;}
    }

   if(sym==true){
       System.out.println("The array is a symetrical array");
   }
   else{
       System.out.println("The array is NOT a symetrical array");
   }
 }
}


