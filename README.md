# codigomorse
/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */
package codigomorse;
import java.util.Scanner; 
/**
 *
 * @author René
 */
public class CodigoMorse {

    /**
     * @param args the command line arguments
     */
   
    public static void main(String[] args) {
        // TODO code application logic her
       Scanner leer=new Scanner(System.in); 
        String p=""; 
         
        System.out.println("Introduce palabra"); 
        p=leer.nextLine(); 
         String m[] = {".----", "..---", "... --", "....-", ".....", 
                "_....", "_ _...", "- - -..", "----.", "-----", ".-", "-...", 
                "-...", "-.-.", "-..", ".", "..-.", "--.", "....", "..", 
                ".---", "-.-", ".-..", "--", "-.", "---", ".--.", "--.-", 
                ".-.", "...", "-", "..-", "...-", ".--", "-..-", "-.--", 
                "--..", ".-", "-...", "-.-.", "-..", ".", "..-.", "--.", 
                "....", "..", ".---", "-.-", ".-..", "--", "-.", "---", ".--.", 
                "--.-", ".-.", "...", "-", "..-", "...-", ".--", "-..-", 
                "-.--", "--..", " ", ".-.-.-", "--..--", "..--..", "---...", 
                "-....-", "!"," "}; 
 
        String l = "1234567890abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ .,?:-!"; 
            int pos=0; 
            String s=""; 
   
        for (int f = 0; f < p.length(); f++) { 
            pos=l.indexOf(p.charAt(f)); 
            s+=m[pos]; 
        } 
        System.out.println(s); 
    } 
    }
    
