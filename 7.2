#include <iostream>
#include <thread>
#include <mutex>
#include <chrono>
#include <random>

class Character {
private:
    std::string name;
    int health;
    int attack;
    std::mutex mtx;

public:
    Character(const std::string& n, int h, int a)
        : name(n), health(h), attack(a) {}

    void takeDamage(int damage) {
        std::lock_guard<std::mutex> lock(mtx);
        health -= damage;
        if (health < 0) health = 0;
    }

    int getAttack() const {
        return attack;
    }

    std::string getName() const {
        return name;
    }

    bool isAlive() const {
        return health > 0;
    }

    void displayStatus() {
        std::lock_guard<std::mutex> lock(mtx);
        std::cout << name << " HP: " << health << std::endl;
    }
};

void fight(Character& attacker, Character& defender) {
    std::random_device rd;
    std::mt19937 gen(rd());
    std::uniform_int_distribution<> damage_dist(1, attacker.getAttack());

    while (attacker.isAlive() && defender.isAlive()) {
        int damage = damage_dist(gen);

        defender.takeDamage(damage);

        std::cout << attacker.getName() << " hits " << defender.getName()
            << " for " << damage << " damage!" << std::endl;

        attacker.displayStatus();
        defender.displayStatus();
        std::cout << "------------------------" << std::endl;

        std::this_thread::sleep_for(std::chrono::seconds(1));

        std::swap(attacker, defender);
    }

    if (attacker.isAlive()) {
        std::cout << attacker.getName() << " wins the battle!" << std::endl;
    }
    else {
        std::cout << defender.getName() << " wins the battle!" << std::endl;
    }
}

int main() {
    Character hero("Hero", 100, 20);
    Character monster("Dragon", 150, 15);

    std::cout << "Battle starts between " << hero.getName()
        << " and " << monster.getName() << "!" << std::endl;

    std::thread battleThread(fight, std::ref(hero), std::ref(monster));

    battleThread.join();

    return 0;
}
