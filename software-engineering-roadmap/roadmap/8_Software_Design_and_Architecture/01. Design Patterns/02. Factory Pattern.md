# Factory Pattern

The Factory pattern provides an interface for creating objects but allows subclasses to alter the type of objects that will be created.

## Key Concepts
- **Object Creation**: The pattern delegates the creation of objects to a factory method.
- **Flexibility**: Allows for easy substitution of different implementations.

## Use Cases
- Creating objects where the exact type may not be known until runtime.
- Implementing complex object creation logic.

## Example Code
### Python
```python
class Car:
    def drive(self):
        pass

class Sedan(Car):
    def drive(self):
        print("Driving a sedan")

class SUV(Car):
    def drive(self):
        print("Driving an SUV")

class CarFactory:
    @staticmethod
    def create_car(car_type):
        if car_type == "sedan":
            return Sedan()
        elif car_type == "suv":
            return SUV()
        else:
            raise ValueError("Unknown car type")
```

## Learning Resources

- [Factory Pattern - Design Patterns](https://www.tutorialspoint.com/design_pattern/factory_pattern.htm)
- [Factory Method Pattern - Refactoring Guru](https://refactoring.guru/design-patterns/factory-method)

## Next Steps

1. Implement the Factory pattern in different scenarios.
2. Explore abstract factories for more complex needs.
