# 18.02
//task  № 1
#include <iostream>
using namespace std;
int main(int argc, char** argv) {
int a = 5;
char b = 36;
const int h = 45;
long b1 = 25661526;
float a1 = 3.3;
double c1 = 3.435435;
volatile int j = 35;
cout << a <<'\n';
cout << b <<'\n';
cout << h <<'\n';
cout << b1 <<'\n';
cout << a1 <<'\n';
cout << c1 <<'\n';
cout << j <<'\n';
    return 0;

}
консоль:
C:\lessons>g++ levelup.cpp

C:\lessons>a
5
$
45
25661526
3.3
3.43544
35
//task  № 2
#include <iostream>
using namespace std;
int main(int argc, char** argv) {
char enum GAME {zero = 48, cross = 88, verticalline = 124, horizonyalline = 95, crossedoutcross };
enum GAME posone, postwo, posthree, posfour, posfive, possix, posseven, poseight, posnine, posten, poseleven, postwelve, posthirteen, posfourteen, posfifteen, possixteen, posseventeen, poseighteen, posnineteen, postwenty, postwentyone;
posone = zero;
postwo = verticalline;
cout << postwo << '\n';
//я посчитал, что в моей игре будут присутствовать 21 положение символов
// получается, что каждому положению будет соответствовать свой символ
    return 0;

}
//task  № 3
#include <iostream>
using namespace std;
int main(int argc, char** argv) {
enum GAME {zero = 48, cross = 88, verticalline = 124, horizonyalline = 95, space = 32, crossedoutcross = 92};
enum GAME posone, postwo, posthree, posfour, posfive, possix, posseven, poseight, posnine, posten, poseleven, postwelve, posthirteen, posfourteen, posfifteen, possixteen, posseventeen, poseighteen, posnineteen, postwenty, postwentyone;
posone = zero;
postwo = verticalline;
string arr[16];
arr[0] = cross;
arr[1] = verticalline;
arr[2] = zero, crossedoutcross;
arr[3] = verticalline;
arr[4] = cross;
cout << arr[0];
cout << arr[1];
cout << arr[2];
cout << arr[3];
cout << arr[4];
arr[5] = space;
arr[6] =cross;
arr[7] = verticalline;
arr[8] = cross;
arr[9] = verticalline;
arr[10] = zero;
arr[11] = space;
arr[12] = zero;
arr[13] = verticalline;
arr[14] = zero;
arr[15] = verticalline;
arr[16] = cross;
cout << arr[5] <<'\n';
cout << arr[6];
cout << arr[7];
cout << arr[8];
cout << arr[9];
cout << arr[10];
cout << arr[11] <<'\n';
cout << arr[12];
cout << arr[13];
cout << arr[14];
cout << arr[15];
cout << arr[16];

    return 0;
консоль:
C:\lessons>g++ levelthree.cpp

C:\lessons>a
X|0|X
X|X|0
0|0|X
C:\lessons>


//task  № 4
#include <iostream>
using namespace std;

enum GAME {zero = 48, cross = 88, verticalline = 124, horizonyalline = 95, space = 32, crossedoutcross = 92};
enum GAME posone, postwo, posthree, posfour, posfive, possix, posseven, poseight, posnine, posten, poseleven, postwelve, posthirteen, posfourteen, posfifteen, possixteen, posseventeen, poseighteen, posnineteen, postwenty, postwentyone;
int main(int argc, char** argv) {
struct crosszero {
std::string name; //имя игрока
int age; // возраст игрока
enum GAME game;
};
struct crosszero a1;
a1.name = "Sergey";
a1.age = 24;
a1.game = zero;
printf("game data: name player: %s, age %d, secondsymbol %c", a1.name.c_str(), a1.age, a1.game);
//данные об игре: имя игрока, возраст, первый вводимый символ(например ноль)
    

    return 0;

}
консоль:
C:\lessons>a
game data: name player: Sergey, age 24, secondsymbol 0
C:\lessons>


//task  № 5
#include <iostream>
using namespace std;
int main(int argc, char** argv) {
union pushups { //количество отжиманий
char name; // название отжиманий
int a; //1 день
int b; //2 день
int c; //3 день
int e; //4 день
};
union practic d;
d.a = 24;
struct test{
char name;
int a : 1;  
int b : 1;
int c : 1;
int e : 1;
}


    return 0;

}
