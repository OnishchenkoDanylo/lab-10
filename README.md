# lab-10(not finished yet)
[diagram.zip](https://github.com/user-attachments/files/18155655/diagram.zip)
/*18. Сформувати список, в якому зберігаються результати сесії групи
(прізвище, середній бал, порядковий номер). Вивести на екран повну
інформацію про студентів. Вивести на екран прізвища студентів, які
отримуватимуть стипендію.*/
#include <iostream>
using namespace std;
int main()
{struct Student
 {char surname[30];
  float mark;
  short n;};
 int k; 
 cout<<"enter the number of students: "; cin>>k;
 cout<<endl;
 Student *sg=new Student[k];
 for (int i = 0; i < k; i++)
 {cout<<"enter the number of student: "; 
  cin>>sg[i].n;
  cout<<"enter the surname of student: "; 
  cin>>sg[i].surname;
  cout<<"enter the medium mark of student: "; 
  cin>>sg[i].mark;}
  for (int i = 0; i < k; i++)
  cout<<sg[i].n<<" "<<sg[i].surname<<"`s medium mark is "<<sg[i].mark<<endl; 
 return 0;}
