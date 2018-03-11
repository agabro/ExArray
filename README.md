public class ExArray {

    public static void main(String[] args) {
        int a = 0 + (int) (Math.random() * ((5 - 0)));
        int b = 5 + (int) (Math.random() * ((10 - 5)));
        int c = 7 + (int) (Math.random() * ((10 - 7)));
        int d = 0 + (int) (Math.random() * ((7 - 0)));
        int[][] checkArray = {{a, c}, {b, d}};

        int x = 0;
        int y = 0;

        for (int i = 0; i < 2; i++) {
            for (int j = 0; j < 2; j++) {
               x = checkArray[i][0];
               y = checkArray[j][1];
               System.out.println("result for x = " + x + " and for y = " + y + " is " + (!(x < 5) && !(y >= 7)));
            }
        }
    }
}
