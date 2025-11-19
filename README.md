# Static_Person_identity-

Author- Shakira Murshida

class Person {

    int age;
    
    String name;
    
    static String university_name = "EUB";//static variable (shared by all objects)

    Person(int age, String name, String university_name) {
        this.age = age;
        this.name = name;
        Person.university_name = university_name;  
        // static variable belongs to the class, so use ClassName.variable
    }

    void display() {
        System.out.println(name + " " + age + " " + university_name);    }
}

class Main {

    public static void main(String[] args) {
        Person p1 = new Person(20, "A", "EUB");
        Person p2 = new Person(21, "B", "EUB");
        Person p3 = new Person(22, "C", "EUB");

        p1.display();
         p2.display();
          p3.display();
    }
}
