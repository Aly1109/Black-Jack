# Black-Jack
Best game you will ever see🤯



import java.util.Scanner;
import java.util.ArrayList;

public class Main {
		    public static void main(String args[]) {
		        Card aceofhearts = new Card(11,"ace","hearts");
		        Card aceofdiamonds = new Card(11,"ace","diamonds");
		        Card aceofspades = new Card(11,"ace","spades");
		        Card aceofclubs = new Card(11,"ace","clubs");
		        Card kingofhearts = new Card(10,"king","hearts");
		        Card kingofdiamonds = new Card(10,"king","diamonds");
		        Card kingofspades = new Card(10,"king","spades");
		        Card kingofclubs = new Card(10,"king","clubs");
		        Card queenofhearts = new Card(10,"queen","hearts");
		        Card queenofdiamonds = new Card(10,"queen","diamonds");
		        Card queenofspades = new Card(10,"queen","spades");
		        Card queenofclubs = new Card(10,"queen","clubs");
		        Card jackofhearts = new Card(10,"jack","hearts");
		        Card jackofdiamonds = new Card(10,"jack","diamonds");
		        Card jackofspades = new Card(10,"jack","spades");
		        Card jackofclubs = new Card(10,"jack","clubs");
		        Card tenofhearts = new Card(10,"ten","hearts");
		        Card tenofdiamonds = new Card(10,"ten","diamonds");
		        Card tenofspades = new Card(10,"ten","spades");
		        Card tenofclubs = new Card(10,"ten","clubs");
		        Card nineofhearts = new Card(9,"nine","hearts");
		        Card nineofdiamonds = new Card(9,"nine","diamonds");
		        Card nineofspades = new Card(9,"nine","spades");
		        Card nineofclubs = new Card(9,"nine","clubs");
		        Card eightofhearts = new Card(8,"eight","hearts");
		        Card eightofdiamonds = new Card(8,"eight","diamonds");
		        Card eightofspades = new Card(8,"eight","spades");
		        Card eightofclubs = new Card(8,"eight","clubs");
		        Card sevenofhearts = new Card(7,"seven","hearts");
		        Card sevenofdiamonds = new Card(7,"seven","diamonds");
		        Card sevenofspades = new Card(7,"seven","spades");
		        Card sevenofclubs = new Card(7,"seven","clubs");    
		        Card sixofhearts = new Card(6,"six","hearts");
		        Card sixofdiamonds = new Card(6,"six","diamonds");
		        Card sixofspades = new Card(6,"six","spades");
		        Card sixofclubs = new Card(6,"six","clubs");
		        Card fiveofhearts = new Card(5,"five","hearts");
		        Card fiveofdiamonds = new Card(5,"five","diamonds");
		        Card fiveofspades = new Card(5,"five","spades");
		        Card fiveofclubs = new Card(5,"five","clubs");
		        Card fourofhearts = new Card(4,"four","hearts");
		        Card fourofdiamonds = new Card(4,"four","diamonds");
		        Card fourofspades = new Card(4,"four","spades");
		        Card fourofclubs = new Card(4,"four","clubs");
		        Card threeofhearts = new Card(3,"three","hearts");
		        Card threeofdiamonds = new Card(3,"three","diamonds");
		        Card threeofspades = new Card(3,"three","spades");
		        Card threeofclubs = new Card(3,"three","clubs");
		        Card twoofhearts = new Card(2,"two","hearts");
		        Card twoofdiamonds = new Card(2,"two","diamonds");
		        Card twoofspades = new Card(2,"two","spades");
		        Card twoofclubs = new Card(2,"two","clubs");
		        
		        
		        ArrayList<Card> deck = new ArrayList<Card>();
		        ArrayList<Card> discard = new ArrayList<Card>();
		        ArrayList<Card> playerhand = new ArrayList<Card>();
		        ArrayList<Card> dealerhand = new ArrayList<Card>();
		        deck.add(aceofhearts);
		        deck.add(kingofhearts);
		        deck.add(aceofdiamonds);
		        deck.add(kingofdiamonds);
		        deck.add(aceofspades);
		        deck.add(aceofclubs);
		        deck.add(kingofspades);
		        deck.add(kingofclubs);
		        deck.add(queenofhearts);
		        deck.add(queenofdiamonds);
		        deck.add(queenofspades);
		        deck.add(queenofclubs);
		        deck.add(jackofhearts);
		        deck.add(jackofdiamonds);
		        deck.add(jackofspades);
		        deck.add(jackofclubs);
		        deck.add(tenofhearts);
		        deck.add(tenofdiamonds);
		        deck.add(tenofspades);
		        deck.add(tenofclubs);
		        deck.add(nineofhearts);
		        deck.add(nineofdiamonds);
		        deck.add(nineofspades);
		        deck.add(nineofclubs);
		        deck.add(eightofhearts);
		        deck.add(eightofdiamonds);
		        deck.add(eightofspades);
		        deck.add(eightofclubs);
		        deck.add(sevenofhearts);
		        deck.add(sevenofdiamonds);
		        deck.add(sevenofspades);
		        deck.add(sevenofclubs);
		        deck.add(sixofhearts);
		        deck.add(sixofdiamonds);
		        deck.add(sixofspades);
		        deck.add(sixofclubs);
		        deck.add(fiveofhearts);
		        deck.add(fiveofdiamonds);
		        deck.add(fiveofspades);
		        deck.add(fiveofclubs);
		        deck.add(fourofhearts);
		        deck.add(fourofdiamonds);
		        deck.add(fourofspades);
		        deck.add(fourofclubs);
		        deck.add(threeofhearts);
		        deck.add(threeofdiamonds);
		        deck.add(threeofspades);
		        deck.add(threeofclubs);
		        deck.add(twoofhearts);
		        deck.add(twoofdiamonds);
		        deck.add(twoofspades);
		        deck.add(twoofclubs);
		        
		        // shuffle  
		        shuffle(deck, discard);
		        
		        
		        Scanner s = new Scanner (System.in);
		        double startingCash=0.0;
		        System.out.println("how much money are you starting with");
		        startingCash=s.nextDouble();
		        int bet = 1;
		    
		        while (bet!=0){
		           System.out.println("how much are you betting? if you want to stop enter 0");
		           bet=s.nextInt();
		           if (bet!=0 && bet <= startingCash){
		               if (deck.size()==0){
		                   shuffle(deck, discard);
		               }
		               draw(deck,playerhand);
		               if (deck.size()==0){
		                   shuffle(deck, discard);
		               }
		               draw(deck,playerhand);
		               if (deck.size()==0){
		                   shuffle(deck, discard);
		               }
		               draw(deck,dealerhand);
		               if (deck.size()==0){
		                   shuffle(deck, discard);
		               }
		               draw(deck,dealerhand);
		               int totval=playerhand.get(0).getValue()+playerhand.get(1).getValue();
		               System.out.println("the dealer top card is "+dealerhand.get(0).getName());
		               System.out.println("in your hand you have ");
		               for (int i = 0 ; i < playerhand.size(); i++){
		                   System.out.println(playerhand.get(i).getName());
		                   
		               }
		               System.out.println("it is worth "+totval+" points");
		               String x="";
		               int c=1;
		               int wq=0;
		               while(!(x.equals("stand"))){
		                   // natiral
		                   if (playerhand.get(0).getValue()+playerhand.get(1).getValue()==21 && dealerhand.get(0).getValue()+dealerhand.get(1).getValue()!=21){
		                       x="stand";
		                       startingCash+= (((double)bet*3)/2);
		                       System.out.println("you got a natural");
		                       System.out.println("your new balance is "+ startingCash);
		                       
		                   }
		                   else if(playerhand.get(0).getValue()+playerhand.get(1).getValue()==21 && dealerhand.get(0).getValue()+dealerhand.get(1).getValue()==21) {
		                	   x="stand";
		                	   System.out.println("you and the dealer both got a natural so it is a tie");
		                   }
		                    else{
		                        System.out.println ("your point total is "+ totval+" do you want to hit or stand?");
		                        x=s.nextLine();
		                        if(x.equals("hit")){
		                            c++;
		                            if (deck.size()==0){
		                            shuffle(deck, discard);
		                            }
		                            draw(deck,playerhand);
		                            System.out.println("you drew a " + playerhand.get(c).getName());
		                            totval+=playerhand.get(c).getValue();
		                       
		                        if (totval>21){                       // if bust
		                            for (int qw=wq; qw<=c; qw++){
		                                if (playerhand.get(qw).getValue()==11){
		                                    System.out.println("your point total is "+ totval+" do you want your " + playerhand.get(qw).getName()+ " to be worth 1 point if so type y if no type n");
		                                    String reduce =s.nextLine();
		                                    wq=qw+1;
		                                    if(reduce.equals("y")){
		                                        totval-=10;
		                                    }
		                                }
		                            }
		                            if (totval>21){
		                                x="stand";
		                                System.out.println("bust");
		                                startingCash-=bet;
		                                System.out.println("your new balance is "+ startingCash);
		                            }
		                            
		                        }
		                       
		                        }
		                    }
		                   
		                   
		               }
		               if (totval<22){
		                    System.out.println("the dealer second card is "+dealerhand.get(1).getName());
		                    int dealerstotal=dealerhand.get(0).getValue()+dealerhand.get(1).getValue();
		                    while (dealerstotal<17){
		                        dealerstotal+=deck.get(0).getValue();
		                        System.out.println("the dealer draws a "+ deck.get(0).getName());
		                        if (deck.size()==0){
		                        shuffle(deck, discard);
		                        }
		                        draw(deck,dealerhand);
		                    }
		                    if (dealerstotal>totval && dealerstotal<22){
		                        startingCash-=bet;
		                        System.out.println("you lost your new balance is "+ startingCash);
		                    }
		                    if (dealerstotal<totval){
		                        startingCash+=bet;
		                        System.out.println("you won your new balance is "+ startingCash);
		                    }
		                    if (dealerstotal==totval){
		                        System.out.println("it's a tie your curent balance is "+ startingCash);
		                    }
		                    if (dealerstotal>21){
		                        startingCash+=bet;
		                        System.out.println("dealer busts you win your new balance is "+startingCash);
		                    }
		                }
		                while(playerhand.size()!=0){
		                    draw(playerhand,discard);
		                }
		                while(dealerhand.size()!=0){
		                    draw(dealerhand,discard);
		                }
		           }
		           // Aly lock 
		           else {
		        	   System.out.println("not enough $");
		           }
		        }
		        s.close();
		    }
		// moves cards from one place to another 
		    public static void draw(ArrayList<Card> from, ArrayList<Card> to){
		          to.add(from.get(0));
		          from.remove(0);
		    }
		    // shuffle
		    public static void shuffle(ArrayList<Card> deck , ArrayList<Card> discard){
		        while (discard.size()!=0){
		            draw(discard, deck);
		        }
		        for (int i=0; i<7; i++){
		            for (int j=0; j<deck.size(); j++){
		                Card temp = deck.get(j);
		                int weeeeeeeeeeeeee=(int)(Math.random()*52);
		                deck.set(j, deck.get(weeeeeeeeeeeeee));
		                deck.set(weeeeeeeeeeeeee, temp);
		            }
		        }
		        System.out.println("deck got shuffeled");
		    }
		    



		

	}


class Card{
    private int Value; 
    private String Type;
    private String Suit; 
    public Card (int val,String t, String s){
        Value = val;
        Type=t;
        Suit=s;
    }
    public int getValue(){
        return Value;
    }
    public String getName(){
        return Type +" of " + Suit;
    }
}
