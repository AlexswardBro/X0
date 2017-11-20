package com.company;

import java.util.Scanner;

public class Main {

    public static void main(String[] args) {

             char[][] field = new char[3][3];
             Scanner scanner = new Scanner(System.in);
       boolean osto = true;

             while(osto = true) {


                 System.out.print("Крестики, введите номер клетки по горизонтали, начиная с 0: ");
                 int a = scanner.nextInt();
                 System.out.print("Крестики, по вертикали: ");
                 int b = scanner.nextInt();
                 field[a][b] = 'x';

                 for (int i = 0; i < 3; i++) {
                     for (int j = 0; j < 3; j++) {
                         System.out.print("{ " + field[i][j] + " } ");
                     }
                     System.out.println();
                 }

                 System.out.print("Нолики, введите номер клетки по горизонтали, начиная с 0: ");
                 int c = scanner.nextInt();
                 System.out.print("Нолики, по вертикали: ");
                 int d = scanner.nextInt();
                 field[c][d] = '0';

                 for (int i = 0; i < 3; i++) {
                     for (int j = 0; j < 3; j++) {
                         System.out.print("{ " + field[i][j] + " }");
                     }
                     System.out.println();
                 }






                 //Горизонтали
                 if ((field[0][0] == field[0][1]) & (field[0][1] == field[0][2]) ) {
                     System.out.println("Победили " + (field[0][0]));
                    osto = false;



                 }
                 else if ((field[1][0] == field[1][1]) & (field[1][1] == field[1][2])) {
                     System.out.println("Победили " + (field[1][0]));
                     osto = false;


                 }
                 else if ((field[2][0] == field[2][1]) & (field[2][1] == field[2][2])) {
                     System.out.println("Победили " + (field[2][0]));
                     osto = false;


                 }


                 //Вертикали

                 if ((field[0][0] == field[1][0]) & (field[1][0] == field[2][0])) {
                     System.out.println("Победили " + (field[0][0]));
                     osto = false;


                 }
                 else if ((field[0][1] == field[1][1]) & (field[1][1] == field[2][1])) {
                     System.out.println("Победили " + (field[0][1]));
                     osto = false;


                 }
                 else if ((field[0][2] == field[1][2]) & (field[1][2] == field[2][2])) {
                     System.out.println("Победили " + (field[0][2]));
                     osto = false;


                 }


                 //Диагонали

                 if ((field[0][0] == field[1][1]) & (field[1][1] == field[2][2])) {
                     System.out.println("Победили " + (field[0][0]));
                     osto = false;

                 }
                 else if ((field[2][0] == field[1][1]) & (field[1][1] == field[0][2])) {
                     System.out.println("Победили " + (field[0][2]));
                     osto = false;

                 }

                 }
             }


             }




