# arraylist


import java.util.ArrayList;
import java.util.Collections;
import java.util.Scanner;

public class Main {
    public static void main(String[] args){
       // while(true)
        System.out.println("1.Add");
        System.out.println("2.remove");
        System.out.println("3.display");
        System.out.println("4.exit");
        Scanner a = new Scanner(System.in);
        ArrayList <Integer>  arrayl = new ArrayList<>();
        while(true){
        int a1 = a.nextInt();
        //switch (true){
        if (a1==1){
            System.out.print("Enter element to add:");
            int b=a.nextInt();
            arrayl.add(b);
            System.out.println("Added Sucessfully!");
            System.out.println(arrayl);
        }
        else if (a1==2){
            System.out.println("Enter element to remove");
            int c=a.nextInt();
            if (arrayl.contains(c)){
            arrayl.remove( Integer.valueOf(c));
            System.out.print("Removed Successfully!");
            System.out.println(arrayl);}
            else
                System.out.println("Value not found!");
        }
        else if (a1==3){
            System.out.print(arrayl);

        }
        else if (a1==4){
            System.out.print("Bye!");
            break;

        }
    }}
}
