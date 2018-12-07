# barbie


/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */
package barbie;

import java.util.Random;

public class Barbie {
    Random r=new Random();
    private String name;
    private int hairLength,outfit,hairColour;

    public Barbie(String name) {
        this.name = name;
    }
    
    public void random(){
        hairColour=r.nextInt(3);
        hairLength=r.nextInt(2);
        outfit=r.nextInt(3);
        if(hairColour==0){
            System.out.println("Hair colour is Red");
        }
        else if(hairColour==1){
            System.out.println("Hair colour is Green");
        }
        else{
            System.out.println("Hair colour is Blue");  
        }
        if(hairLength==0){
            System.out.println("Hair length is short");
        }
        else{
            System.out.println("Hair length is long");
        }
        if(outfit==0){
            System.out.println("Outfit is shirt");
        }
        else if(outfit==1){
            System.out.println("Outfit is dress");
        }
        else{
            System.out.println("Outfit is Jacket");
        }
        
    }
    public void cutHair(){
        if(hairLength==0){
            System.out.println("Hair is already short.");
        }
        else if(hairLength==1){
        
        
        
        
        
        
        
        
        
        BARBIE2
        
        
        
        /*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */
package barbie;

/**
 *
 * @author izzati
 */
public class TesterBarbie {
    public static void main(String[] args) {
        Barbie b=new Barbie("Lisa");
        b.display();
        b.random();
        b.cutHair();
        
    }
}










POKEMON1


/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */
package pokemon;

/**
 *
 * @author Fortune
 */
public class TestPokemon {
    public static void main(String[] args){
        Pokemon p = new Pokemon("meepo123","meepo","water");
        System.out.println("Level 1");
        p.random();
        p.level();
        System.out.println();
        p.display();
        
        
        
    }
}






POKEMON2



/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */
package pokemon;

import java.util.Random;

public class Pokemon {
    Random r=new Random();
    private String ID,name,type;
    private int hp,attack,defense,speed,special,level=2;
    private int newhp,newAttack,newDefense,newSpeed,newSpecial;
    

    public Pokemon(String ID, String name, String type) {
        this.ID = ID;
        this.name = name;
        this.type = type;       
    }
    
    public void random(){
        hp=r.nextInt(11)+15;
        System.out.println("Current hitpoint: "+hp);
        attack=r.nextInt(8)+10;
        System.out.println("Current attack: "+attack);
        defense=r.nextInt(8)+10;
        System.out.println("Current defense: "+defense);
        speed=r.nextInt(11)+5;
        System.out.println("Current speed: "+speed);
        special=r.nextInt(6)+5;
        System.out.println("Current special: "+special);
    }
    
    public void level(){
//        level=level+1;
        while(level<=3){
            System.out.println("Level "+level);
        hp=hp+r.nextInt(4)+2;
        System.out.println("New Hitpoint: "+ hp);
        attack=r.nextInt(3)+1+attack;
        System.out.println("New Attack: "+ attack);
        defense=r.nextInt(3)+1+defense;
        System.out.println("New Defense: "+ defense);
        speed=r.nextInt(3)+1+speed;
        System.out.println("New Speed: "+ speed);
        special=r.nextInt(3)+1+special;
        System.out.println("New Special: "+ special);
        level=level+1;
        }
    }
    
    public void display(){
        System.out.println("ID: "+ID);
        System.out.println("Name: "+name);
        System.out.println("Element type: "+type);
    }
    }
