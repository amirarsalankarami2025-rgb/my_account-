lass Car {
    // Fields (attributes)
    String rand;
    String color;
    int year;

    // Constructo
    Car(String brand, String color, int year) {
        this.brand = brand;
        this.color = color;
        this.year = year;
    }

    // Method
    void drive() {
        System.out.println("The " + color + " " + brand + " from " + year + " is driving!");
    }
}

public class CarDemo {
    public static void main(String[] args) {
        // Create objects
        Car car1 = ew Car("Toyota", "Red", 2020);
        Car car2 = new Car("BMW", "Black", 2022);

        // Call methods
        car1.drive();
        car2.drive();
    }
}
