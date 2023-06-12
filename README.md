public class MainChallenge {
    public static void main(String[] args){

        boolean gameOver = true;
        int myscore = 800;
        int levelcomplete = 5;
        int bounus = 100;

//
      int highscore = calculatescore(gameOver, myscore, levelcomplete, bounus);
      System.out.println("The high score is" + highscore);

        myscore = 10000;
        levelcomplete = 8;
         bounus = 200;


System.out.println("The second highest score is " +
      calculatescore(gameOver, myscore, levelcomplete, bounus));
       }

       public static int calculatescore(boolean gameOver, int myscore, int levelcomplete, int bounus){

//
           int finalscore =myscore;
//
           if(gameOver == true){
               finalscore +=(levelcomplete * bounus);

           }
           return finalscore;
       }

        }


