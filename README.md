# MohammadSayed02Repository
uses of & operator:

1-p_to_y = &y;/*If p_to_y is defined as a pointer to an int and y as an int, the following expression assigns the address of the variable y to the pointer p_to_y*/

2-/*The ampersand symbol & is used in C++ as a reference declarator in addition to being the address operator. The meanings are related but not identical.*/
int target;
int &rTarg = target;  // rTarg is a reference to an integer.
// The reference is initialized to refer to target.

3-/*The & (bitwise AND) in C or C++ takes two numbers as operands and does AND on every bit of two numbers. The result of AND is 1 only if both bits are 1. */
int x=5;//101
int y=4;//100
cout<<(x&y); //it'll print 4 not 1 as AND logic operator

4-bool x,y;
x=true;
y=false;
cout<<x&&y<<endl;// print false as a result of AND logic operator

///////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////

uses of const:

1-/*declarition of constant variables which we can't operate on later*/

const int x=25;

x=20;//Error because this variable is constant


2-/*declaration of the constant pointer which point to a variable ,so it can't be changed*/

int x=5;

int y=6;

const int* p=&x;

p=&y;//Error

p++;//Error


3-int T(const int &x){

return x++;

}//Error x is a constant variable called by reference

4-int T (const int x){

return x++;

}// Error x is a constant variable