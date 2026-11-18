# Creature Battle Project (OOP + Git Branching Practice)

This project is designed to help me learn **object-oriented programming** in Python — especially **inheritance** — while also practicing key **Git concepts** like branching, merging, conflict resolution, and version history.

I began with a base class (`Creature`) on `main` and created additional subclasses (`FlyingCreature`, `SwimmingCreature`, and `FireCreature`) on separate Git branches to simulate a real development workflow.

---

## Learning Objectives

### Python / OOP
- Understand and implement **classes**
- Use **inheritance** to extend behaviors
- Override and extend methods (e.g., `attack()`)
- Practice writing simple test code in `main`

### Git / Version Control
- Create and switch branches
- Merge branches into `main`
- Resolve merge conflicts
- View commit history (`git log --graph --all`)

---

## Project Structure

```text
oop_creature_code/
│
├── creature_simulation.py   # Base class (Creature) + subclasses + test cases
└── README.md                # Project documentation
```

---

## Implemented Classes

- **`Creature` (Base Class):** Defines core attributes (`name`, `hp`, `attack_power`) and basic methods (`attack()`, `is_alive()`, `__str__()`).
- **`FlyingCreature(Creature)`:** Adds `altitude` and `fly_to()`, and overrides `attack()` for aerial attacks.
- **`SwimmingCreature(Creature)`:** Adds `depth` and `dive_to()`, and overrides `attack()` for underwater attacks.
- **`FireCreature(Creature)`:** Adds `fire_level` (0–100) and `emit_fire()`, and overrides `attack()` for flame-based attacks.

---

## How to Test and Run

1. **Navigate to the project directory:**
   ```bash
   cd oop_creature_code
   ```

2. **Run the simulation and test cases** using Python 3:
   ```bash
   python creature_simulation.py
   ```
   The script automatically runs the test cases inside the `if __name__ == "__main__":` block to verify initialization, HP reduction, `is_alive()` status, and overridden `attack()` outputs for all classes.

3. **View the Git branching and merge history:**
   ```bash
   git log --all --graph
   ```