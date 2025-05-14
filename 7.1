#include <iostream>
#include <fstream>
#include <vector>
#include <string>
#include <stdexcept>

class Character {
private:
    std::string name;
    int health;
    int level;

public:
    Character(const std::string& n, int h, int lvl)
        : name(n), health(h), level(lvl) {}

    void save(std::ofstream& file) const {
        file << name << '\n' << health << '\n' << level << '\n';
    }

    static Character load(std::ifstream& file) {
        std::string name;
        int health, level;

        std::getline(file, name);
        file >> health >> level;
        file.ignore();

        return Character(name, health, level);
    }

    void displayInfo() const {
        std::cout << "Name: " << name << ", Health: " << health
            << ", Level: " << level << std::endl;
    }
};

void saveCharactersToFile(const std::vector<Character>& characters,
    const std::string& filename) {
    std::ofstream file(filename);
    if (!file) {
        throw std::runtime_error("Failed to open file for writing");
    }

    file << characters.size() << '\n'; 
    for (const auto& character : characters) {
        character.save(file);
    }
}

std::vector<Character> loadCharactersFromFile(const std::string& filename) {
    std::ifstream file(filename);
    if (!file) {
        throw std::runtime_error("Failed to open file for reading");
    }

    std::vector<Character> characters;
    int count;
    file >> count;
    file.ignore(); 

    for (int i = 0; i < count; ++i) {
        characters.push_back(Character::load(file));
    }

    return characters;
}

int main() {
    try {
        std::vector<Character> characters = {
            Character("Hero", 100, 5),
            Character("Mage", 80, 7),
            Character("Warrior", 120, 4)
        };

        saveCharactersToFile(characters, "characters_save.txt");
        std::cout << "Characters saved to file.\n";

        auto loadedCharacters = loadCharactersFromFile("characters_save.txt");
        std::cout << "\nLoaded characters:\n";

        for (const auto& character : loadedCharacters) {
            character.displayInfo();
        }

    }
    catch (const std::exception& e) {
        std::cerr << "Error: " << e.what() << std::endl;
        return 1;
    }

    return 0;
}
