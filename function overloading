#include <iostream>
using namespace std;

class RedBull {
public:
    void drink() {
        cout << "Red Bull Classic      Caffeine: 80mg       Sugar: 27g" << endl;
    }

    void drink(string flavour) {
        cout << "Red Bull " << flavour << endl;
    }

    void drink(string flavour, int caffeine) {
        cout << "Red Bull " << flavour 
             << "      Caffeine: " << caffeine << "mg" << endl;
    }

    void drink(string flavour, int caffeine, int sugar) {
        cout << "Red Bull " << flavour 
             << "      Caffeine: " << caffeine << "mg"
             << "      Sugar: " << sugar << "g" << endl;
    }
};

int main() {
    RedBull rb;

    rb.drink();
    rb.drink("Sugarfree");
    rb.drink("Tropical", 80);
    rb.drink("Blue Edition", 80, 27);

    return 0;
}



//Expected Output



Red Bull Classic      Caffeine: 80mg   Sugar: 27g
Red Bull Sugarfree    
Red Bull Tropical     Caffeine: 80mg
Red Bull Blue Edition Caffeine: 80mg   Sugar: 27g
