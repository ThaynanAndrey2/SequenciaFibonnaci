# SequenciaFibonnaci
Verificar uma Sequência Fibonacci utilziando C++

#include <iostream>
using namespace std;

int main() {
    int n, t1 = 0, t2 = 1, prox = 0;

    cout << "Coloque o numero de termos: ";
    cin >> n;

    cout << "Sequencia de Fibonacci: ";

    for (int i = 1; i <= n; ++i) {
        if(i == 1) {
            cout << t1;
            continue;
        }
        if(i == 2) {
            cout << ", " << t2;
            continue;
        }
        prox = t1 + t2;
        t1 = t2;
        t2 = prox;
        
        cout << ", " << prox;
    }

    return 0;
}
