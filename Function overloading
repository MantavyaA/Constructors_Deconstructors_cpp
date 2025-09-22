#include <iostream>
using namespace std;

class Distance {
    int km, m;
public:
    Distance(int k=0, int mm=0) {
        km = k;
        m = mm;
    }

    Distance operator + (Distance d) {
        Distance res;
        res.km = km + d.km;
        res.m = m + d.m;

        if (res.m >= 1000) {
            res.km += res.m / 1000;
            res.m = res.m % 1000;
        }
        return res;
    }

    void display() {
        cout << km << " km " << m << " m" << endl;
    }
};

int main() {
    Distance d1(5, 750);   
    Distance d2(3, 500);   

    Distance d3 = d1 + d2;   
    d3.display();   

    return 0;
}



//Expected Output
9 km 250 m
