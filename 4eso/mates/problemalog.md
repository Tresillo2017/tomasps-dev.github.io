# Problema Logaritmo
```c++
#include <bits/stdc++.h>
using namespace std;

int main()
{
    float res = 1;
    float ren = log10(2);
    float ren1 = log10(3);
    for(int i = 3; i <= 128; i++)
    {
        res = res * (ren1/ren);
        ren = ren1;
        ren1 = log10(i+1);
    }
    cout << res << endl;
}
```
