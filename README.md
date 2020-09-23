<div align="center">

## A quadratic equation solver


</div>

### Description

This program solves quadratic equations for you. All you have to do is enter the value of a, b, and c. I wanted to check my homework for my math class, so i made this program mainly overnight.
 
### More Info
 
A,B,C


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Mauricio Rossi](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/mauricio-rossi.md)
**Level**          |Intermediate
**User Rating**    |4.7 (28 globes from 6 users)
**Compatibility**  |C\+\+ \(general\), Microsoft Visual C\+\+, Borland C\+\+
**Category**       |[Math](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/math__3-12.md)
**World**          |[C / C\+\+](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/c-c.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/mauricio-rossi-a-quadratic-equation-solver__3-9338/archive/master.zip)





### Source Code

```
#include <cmath>
#include <iostream>
char e;
using namespace std;
void calculate();
void ask();
int main() {
cout << "\t   Quadratic Equation Solver\n\t\t by Mauricio Rossi\n\n";
cout << "This program will solve quadratic equations for you.\n";
cout << "Just enter the values of A,B, and C of a qudratic equation.\n";
calculate();
return 0;
}
void ask(){
cout << "Would you like to solve another equation Y/N?";
cin >> e;
if (e == 'y' || e == 'Y'){
calculate();
}
if(e == 'n' || e == 'N'){ }
else {
cout << "Invalid command\n";
system("PAUSE");
}
}
void calculate(){
double a,b,c,a1,a2,a3,nb,sb,divider,result1,result2,div,div2;
cout << "Enter value of A\t";
cin >> a;
cout << "Enter value of B\t";
cin >> b;
cout << "Enter value of C\t";
cin >> c;
nb = -b;
sb = pow(b, 2);
a1 = -4 * a * c;
a2 = sb + a1;
a3 = sqrt(a2);
result1 = nb - a3;
result2 = nb + a3;
divider = 2 * a;
div = result1 / divider;
div2 = result2 / divider;
cout << "The answer is:\t(" << div << "," << div2 << ")" << "\n";
ask();
}
```

