# Black-Jack
Best game you will ever see🤯

import java.util.Scanner;

public class MyClass {
    public static void main(String args[]) {
        Card aceofhearts = new card(1,ace,hearts);
        Card aceofdiamonds = new card(1,ace,diamonds);
        Card aceofspades = new card(1,ace,spades);
        Card aceofclubs = new card(1,ace,clubs);
        Card kingofhearts = new card(10,king,hearts);
        Card kingofdiamonds = new card(10,king,diamonds);
        Card kingofspades = new card(10,king,spades);
        Card kingofclubs = new card(10,king,clubs);
        Card queenofhearts = new card(10,queen,hearts);
        Card queenofdiamonds = new card(10,queen,diamonds);
        Card queenofspades = new card(10,queen,spades);
        Card queenofclubs = new card(10,queen,clubs);
        Card jackofhearts = new card(10,jack,hearts);
        Card jackofdiamonds = new card(10,jack,diamonds);
        Card jackofspades = new card(10,jack,spades);
        Card jackofclubs = new card(10,jack,clubs);
        Card tenofhearts = new card(10,ten,hearts);
        Card tenofdiamonds = new card(10,ten,diamonds);
        Card tenofspades = new card(10,ten,spades);
        Card tenofclubs = new card(10,ten,clubs);
        Card nineofhearts = new card(9,nine,hearts);
        Card nineofdiamonds = new card(9,nine,diamonds);
        Card nineofspades = new card(9,nine,spades);
        Card nineofclubs = new card(9,nine,clubs);
        Card eightofhearts = new card(8,eight,hearts);
        Card eightofdiamonds = new card(8,eight,diamonds);
        Card eightofspades = new card(8,eight,spades);
        Card eightofclubs = new card(8,eight,clubs);
        Card sevenofhearts = new card(7,seven,hearts);
        Card sevenofdiamonds = new card(7,seven,diamonds);
        Card sevenofspades = new card(7,seven,spades);
        Card sevenofclubs = new card(7,seven,clubs);    
        Card sixofhearts = new card(6,six,hearts);
        Card sixofdiamonds = new card(6,six,diamonds);
        Card sixofspades = new card(6,six,spades);
        Card sixofclubs = new card(6,six,clubs);
        Card fiveofhearts = new card(5,ace,hearts);
        Card fiveofdiamonds = new card(5,ace,diamonds);
        Card fiveofspades = new card(5,ace,spades);
        Card fiveofclubs = new card(5,ace,clubs);
        Card fourofhearts = new card(4,four,hearts);
        Card fourofdiamonds = new card(4,four,diamonds);
        Card fourofspades = new card(4,four,spades);
        Card fourofclubs = new card(4,four,clubs);
        Card threeofhearts = new card(3,three,hearts);
        Card threeofdiamonds = new card(3,three,diamonds);
        Card threeofspades = new card(3,three,spades);
        Card threeofclubs = new card(3,three,clubs);
        Card twoofhearts = new card(2,two,hearts);
        Card twoofdiamonds = new card(2,two,diamonds);
        Card twoofspades = new card(2,two,spades);
        Card twoofclubs = new card(2,two,clubs);
    
    
    
    
        Scanner s = new Scanner (System.in);
        int bet = 0;
        System.out.println("how much are you betting?");
        bet=s.nextInt();
    
    
    
    }
}
public class Card{
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
