
## Abstract interface for any Car type
``` c++
class Car {
public:
// Pure virtual methods - no implementation here
virtual void startEngine() = 0;
virtual void shiftGear(int newGear) = 0;
virtual void accelerate() = 0;
virtual void brake() = 0;
virtual ~Car() {}
};

- Benefits of Abstraction

1. Simplified Interfaces: Clients focus on what an object does, not how it does it.
2. Ease of Maintenance: Internal changes (e.g., switching from a V6 to an electric motor)
don’t affect client code.
3. Code Reuse: Multiple concrete classes can implement the same abstract interface (e.g.,
SportsCar, SUV, ElectricCar).
4. Reduced Complexity: Large systems are easier to reason about when broken into
abstract modules.

 - Encapsulation Benefits
1. Robustness: Prevents accidental or malicious misuse of internal state.
2. Maintainability: Internal changes (e.g., adding new constraints) do not ripple into client
code.
3. Clear Contracts: Clients interact only via well-defined methods (the public API).
4. Modularity: Code is organized into self-contained units, easing testing and reuse

```