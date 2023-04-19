# Nested-class-
class Outer{

    int x=3, y=4;

    void out(){

        System.out.println("Outer class m1");

    }

    class Inner{

        int a=1, b=2;

        void inn(){

            System.out.println("Inner class m2");

            System.out.println(a+b);

            System.out.println(x+y);

        }

    }

}

class Code{

    public static void main(String... args){

        Outer o=new Outer();

        o.out();

      Outer.Inner i=o.new Inner();

      i.inn();

    }

}

/*

Outer class m1

Inner class m2

3

7

 */
