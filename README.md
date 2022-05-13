# Black-Jack
Best game you will ever see🤯

public class MyClass {
    public static void main(String args[]) {
    Card aceofhearts = new card(1,ace,hearts);
    Card aceofdiamonds = new card(1,ace,diamonds);
    Card aceofspades = new card(1,ace,spades);
    Card aceofclubs = new card(1,ace,clubss);

    
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
