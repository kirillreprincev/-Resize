#include <iostream>


using namespace std;

int resize(int n) {
    int old_n = 55;
    int* ptr = new int[old_n];
    int* ptr2 = new int[n];
    if (n > old_n) {
        for (int i = 0; i < old_n; i++) {
            ptr[i] = ptr2[i];
        }
    }
    else if (n == 0) {
        delete [] ptr;
        cout << " n = 0 " << endl;
    }
    else if (n < old_n, n > 0) {
        for (int i = 0; i < n; i++) {
            ptr[i] = ptr2[i];
        }
    }
    else {
        cout << "Error 0 - Выход за пределы массива" << endl;
    }
}

int main() {
    resize(n);
    return 0;
}
