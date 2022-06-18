# MatrisTranspozu

import java.util.Arrays;

public class Main {
    
    public static void main(String[] args) {
        int[][] list = {
                {1, 2, 3},
                {4, 5, 6}
        };

        int[][] tlist = new int[list[0].length][list.length];

        for (int i = 0; i < tlist.length; i++) {

            for (int j = 0; j < tlist[0].length; j++) {

                tlist[i][j] = list[j][i];
            }
        }

        for (int i=0;i<tlist.length;i++){
            for (int j=0;j<tlist[i].length;j++){
                System.out.print(tlist[i][j] + " ");
            }
            System.out.println(" ");
        }
    }
}
