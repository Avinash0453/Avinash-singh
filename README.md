# Avinash-singh
class Animal {
    public void makeSound() {
         System.out.println("Some generic animal sound");
    }
}
class Dog extends Animal {
    @Override
    public void makeSound() {
        System.out.println("Woof! Woof!");
    }
}
class Cat extends Animal {
    @Override
    public void makeSound() {
        System.out.println("Meow! Meow!");
    }
}
public class PolymorphismDemo {
    public static void main(String[] args) {
        Animal animal1 = new Dog();
        Animal animal2 = new Cat();
        System.out.println("Animal reference holding Dog object:");
        animal1.makeSound();
        System.out.println("\nAnimal reference holding Cat object:");
        animal2.makeSound(); 
        Animal[] animals = {new Dog(), new Cat()};

        System.out.println("\nDemonstrating polymorphism in an array:");
        for (Animal animal : animals) {
            animal.makeSound(); // Output: Woof! Woof! and Meow! Meow!
        }
    }
}

 
