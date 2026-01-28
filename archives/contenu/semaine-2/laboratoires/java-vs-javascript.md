# Java vs JavaScript

## Intention

Dans ce premier laboratoire, il s'agit de prendre le temps de lire les deux exemples de code (Java et JavaScript) et de faire le lien avec les concepts qui ont été abordés dans l'[introduction au langage](../../semaine-1/theorie-et-concept/introduction.md).

```javascript
// JavaScript: Handling an array of car objects

// Array of car objects
const cars = [
    { make: 'Toyota', model: 'Camry', year: 2020 },
    { make: 'Honda', model: 'Civic', year: 2018 },
    { make: 'Ford', model: 'Mustang', year: 2021 },
    { make: 'Chevrolet', model: 'Malibu', year: 2019 }
];

// Accessing and printing each car's details
cars.forEach(car => {
    console.log(`Make: ${car.make}, Model: ${car.model}, Year: ${car.year}`);
});

// Filtering cars by a specific year
const carsAfter2019 = cars.filter(car => car.year > 2019);
console.log('Cars made after 2019:', carsAfter2019);

// Finding a car by model
const civic = cars.find(car => car.model === 'Civic');
console.log('Found car:', civic);
```

```java
// Java: Handling an array of car objects

import java.util.ArrayList;
import java.util.List;

class Car {
    String make;
    String model;
    int year;

    // Constructor
    Car(String make, String model, int year) {
        this.make = make;
        this.model = model;
        this.year = year;
    }

    // Method to print car details
    void printCarDetails() {
        System.out.println("Make: " + make + ", Model: " + model + ", Year: " + year);
    }
}

public class Main {
    public static void main(String[] args) {
        // List of car objects
        List<Car> cars = new ArrayList<>();
        cars.add(new Car("Toyota", "Camry", 2020));
        cars.add(new Car("Honda", "Civic", 2018));
        cars.add(new Car("Ford", "Mustang", 2021));
        cars.add(new Car("Chevrolet", "Malibu", 2019));

        // Accessing and printing each car's details
        for (Car car : cars) {
            car.printCarDetails();
        }

        // Filtering cars by a specific year
        List<Car> carsAfter2019 = new ArrayList<>();
        for (Car car : cars) {
            if (car.year > 2019) {
                carsAfter2019.add(car);
            }
        }
        System.out.println("Cars made after 2019:");
        for (Car car : carsAfter2019) {
            car.printCarDetails();
        }

        // Finding a car by model
        Car foundCar = null;
        for (Car car : cars) {
            if (car.model.equals("Civic")) {
                foundCar = car;
                break;
            }
        }
        System.out.println("Found car:");
        if (foundCar != null) {
            foundCar.printCarDetails();
        } else {
            System.out.println("Car not found.");
        }
    }
}

```

## Todo:

* [ ] Comment les variables sont-elles déclarées ?
* [ ] Observez la manière dont les voitures sont modélisées...
  * [ ] Comment les deux langages les représentent (structure, tableau, objet).
  * [ ] Comment les deux langages y accèdent.
  * [ ] Comment les deux languages les affichent.
* [ ] Quelles différences de sythaxes mettez-vous en évidence ?
  * [ ] Majuscule, minuscule,
  * [ ] Fin de ligne,
  * [ ] Alignement et indentation.
