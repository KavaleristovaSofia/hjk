#include <iostream>
#include <string>

class Weapon {
private:
    std::string name;
    int damage;
    float weight;

public:
    Weapon(const std::string& n, int d, float w) : name(n), damage(d), weight(w) {}

    // Перегрузка оператора +
    Weapon operator+(const Weapon& other) const {
        std::string newName = name + "+" + other.name;
        int newDamage = damage + other.damage;
        float newWeight = weight + other.weight;
        return Weapon(newName, newDamage, newWeight);
    }

    // Перегрузка оператора >
    bool operator>(const Weapon& other) const {
        return damage > other.damage;
    }

    // Перегрузка оператора <<
    friend std::ostream& operator<<(std::ostream& os, const Weapon& weapon) {
        os << "Weapon: " << weapon.name << ", Damage: " << weapon.damage
            << ", Weight: " << weapon.weight << " kg";
        return os;
    }
};

int main() {
    Weapon sword("Steel Sword", 25, 3.5);
    Weapon bow("Long Bow", 20, 2.1);
    Weapon axe("Battle Axe", 30, 5.2);

    // Демонстрация перегрузки оператора +
    Weapon combined = sword + bow;
    std::cout << "Combined weapon: " << combined << std::endl;

    // Демонстрация перегрузки оператора >
    std::cout << "\nWeapon comparison:\n";
    std::cout << sword << (sword > bow ? " > " : " <= ") << bow << std::endl;
    std::cout << axe << (axe > sword ? " > " : " <= ") << sword << std::endl;
    std::cout << bow << (bow > axe ? " > " : " <= ") << axe << std::endl;

    return 0;
}
