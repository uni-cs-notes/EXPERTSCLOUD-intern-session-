# Assignment # 2 ✅

> Q1📝
```
#include <iostream>
using namespace std;

int main(){
 int bonus , salery , service;
    cout<<"enter the amount of service spend in the company : ";
    cin >> service;
    cout<<"enter ur salery :";
    cin>>salery;
   if (salery == 0 && service == 0){
    cout<<"ERROR > invaild amout";
   }
     bonus = (salery * service) /100;

    cout<<"total bonus : "<<bonus;
 return 0;
 }
```
> Q2📝
```
 #include <iostream>
 using namespace std;

 int main(){
    /* 
     Below 25 - F
	 25 to 45 - E
	 45 to 50 - D
	 50 to 60 - C
	 60 to 80 - B
	 Above 80 - A
    */
   int grade = 0;
   cout << "enter ur score (0 - 100): ";
   cin >> grade;
   if (grade <= 25){
    cout<<"grade > F";
   } 
   else if (grade <= 45){
        cout<<"grade > E";
   }
   else if (grade <= 50){
    cout<<"grade > D";
   } 
   else if (grade <= 60){
    cout<<"grade > C";
   }
   else if (grade <= 80){
    cout<<"grade > B";
   }
   else{
    cout<<"grade > A";
   }
    return 0;
   }
```
> Q3📝
```
#include <iostream>
using namespace std;   
int main(){
 int num1 , num2 ;
 cout<<"enter integer : ";
 cin>>num1;
 cout<<"enter integer : ";
 cin>>num2;
 if ( num1 > num2){
   cout<<"integer 1 is greater than integer 2 ";
 }else if (num2 > num1){
    cout<<"integer 2 is greater than integer 1 ";
 }
return 0;
}
```
> Q4📝
```
#include <iostream>
using namespace std;
int main() {
int age;
cout<<"enter your age:";
cin>>age;
if (age>=14){
    cout<<"your a teen!"<<endl;
}
    else if (age<14)
    cout<<"your a chlid!"<<endl;

    return 0;
}
```
> Q5📝
```
#include <iostream>
using namespace std;
int main(){
    int num1 , num2 ;
    char keys;
    cout<<"enter your 1st value:";
    cin>>num1;
    cout<<"enter your 2nd value:";
    cin>>num2;
    cout<<"enter your operation:";
    cin>>keys;
    switch (keys){
        case '+': cout<<"answer:"<<(num1+num2); break;
        case '-': cout<<"answer:"<<(num1-num2); break;
        case '*': cout<<"answer:"<<(num1*num2); break;
        case '/': cout<<"answer:"<<(num1/num2); break;
        default : cout<<"invalid operation!!"; break;
    }
  return 0;
}
```
> Q6📝
```
#include <iostream>
using namespace std;
int main(){
int year;
cout<<"enter year:";
cin>>year;
if ((year%4==0) && (year%100!=0))  
    cout<<"ur year is a leap year";
else
    cout<<"ur year is not a leap year";
return 0;
}
```
> Q7📝
```
#include <iostream>
using namespace std;

int main(){
int attendance , classHeld , totalAttendance = 0;
cout<<"enter amout of classes Held > ";
cin>>classHeld;
cout<<"enter the amout of classes attended > ";
cin>>attendance;

totalAttendance = (attendance / classHeld)*100; 
if (totalAttendance < 75){
    cout<<"ur eligible to sit in exam ";
} else{
    cout<<"ur not eligible for exam";
}
return 0;
}
```
> Q8 📝
```
#include <iostream>  // modification to Q7 
using namespace std;

int main(){
int attendance , classHeld , totalAttendance = 0;
char answer;
cout<<"enter amout of classes Held > ";
cin>>classHeld;
cout<<"enter the amout of classes attended > ";
cin>>attendance;

totalAttendance = (attendance / classHeld)*100;
 cout<<"do u have any medical condition ! > ('y' or 'n' for answering) \n >";  
 cin>>answer;
  if (answer == 'y' || answer == 'Y'){
    cout<<"ur eligible ";
  } if(answer == 'n' || answer == 'N'){ 
                                              // i have set the program as if a student have a medical condition soo he'll 
                                              // automatically set in exam > the one with no medical condition has to goo through rest 
                                              // process
 if(totalAttendance < 75){
    cout<<"ur not eligible to sit in exam ";
}else{
    cout<<"ur eligible for exam";
}
  } 
return 0;
}
```
> Q9📝
```
#include <iostream>
using namespace std;
int main ()
{
int day;
      cout<<"DAYS OF THE WEEK"<<endl;
      cout<<"1.(sunday)"<<endl;
      cout<<"2.(monday)"<<endl;
      cout<<"3.(tuesday)"<<endl;
      cout<<"4.(wednesday"<<endl;
      cout<<"5.(thursday)"<<endl;
      cout<<"6.(friday)"<<endl;
      cout<<"7.(saturday)"<<endl;
      cout<<"Enter the serial No (to run the code) \n >> ";
      cin>>day;
      switch (day){
          case 1: cout<<" it's Sunday"<<endl;
          break;
          case 2: cout<<"it's Monday"<<endl;
          break;
          case 3: cout<<"it's Tuesday"<<endl;
          break;
          case 4: cout<<"it's Wednesday"<<endl;
          break;
           case 5: cout<<"it's Thursday"<<endl;
          break;
           case 6: cout<<"it's Friday"<<endl;
          break;
           case 7:cout<<"it's Saturday"<<endl;
          break;
          default: cout<<" ERROR >> 'not a Day!!' "<<endl;
          break;
   }
return 0;
 }
```
> Q10📝
```
#include <iostream>
using namespace std;
int main()
{
    int month;
    cout<<"DAYS IN A MONTHS \N ENTER UR MONTH TO DETERMINE THE DAYS IN THEM!!"<<endl;
    cout<<"1.jan"<<endl;
    cout<<"2.feb"<<endl;
    cout<<"3.march"<<endl;
    cout<<"4.april"<<endl;
    cout<<"5.may"<<endl;
    cout<<"6.june"<<endl;
    cout<<"7.july"<<endl;
    cout<<"8.aug"<<endl;
    cout<<"9.sep"<<endl;
    cout<<"10.oct"<<endl;
    cout<<"11.nov"<<endl;
    cout<<"12.dec"<<endl;
    cout<<"enter ur month number"<<endl;
    cin>>month;
    switch(month){
        case 1: cout <<">> 31 days"<<endl;
        break;
        case 2: cout <<">> 28 \ sometimes 29 if leap year"<<endl;
        break;
        case 3: cout <<">> 31 days"<<endl;
        break;
        case 4: cout <<">> 30 days"<<endl;
        break;
        case 5: cout <<">> 31 days"<<endl;
        break;
        case 6: cout <<">> 30 days"<<endl;
        break;
        case 7: cout <<">> 31 days"<<endl;
        break;
        case 8: cout <<">> 31 days"<<endl;
        break;
        case 9: cout <<">> 30 days"<<endl;
        break;
        case 10: cout <<">> 31 days"<<endl;
        break;
        case 11: cout <<">> 30 days"<<endl;
        break;
        case 12: cout <<">> 31 days"<<endl;
        break;
        default: cout<<"NOT a month ";
        break;
    }
}
```
> Q11📝
```
#include <iostream>
using namespace std;

int main(){
    char answer;
    cout<<"enter an alphabet > ";
    cin>> answer;
     switch(answer){
         case 'a' : cout<<"vowel";
         break; 
         case 'e' : cout<<"vowel";
         break; 
         case 'i' : cout<<"vowel";
         break; 
         case 'o' : cout<<"vowel";
         break; 
         case 'u' : cout<<"vowel";
         break; 
         default:cout<<"consonant";
        }             
}
```
> Q12📝
```
#include <iostream>
using namespace std;

int main(){
    int num1 , num2;
    cout<<"enter integer 1 > ";
    cin>>num1;
    cout<<"enter integer 2 > ";
    cin>>num2;
    switch(num1 > num2){    
        case 1: cout<<"integer 1 is greater than integer 2";
            break;
        
        default: cout<<"integer 2 is greater than integer 2";
            break;
        }
     if (num1 == num2){
      cout<<"there equal";
   }
}
```
> Q13📝
```
#include <iostream>
using namespace std;

int main(){
    int num;
    cout<<"enter an integer > ";
    cin>>num;
   switch(num % 2){
    case 1 : cout<<" the integer is even ";
    break;
    default : cout<<"the integer is Odd";
   }
}
```
> Q14📝
```
#include <iostream>
using namespace std;

int main(){
int num;
cout<<"enter the number of ur choice";
if (num == 0){
    cout<<"its a zero";
    switch(num >= 1){
        case 1 : cout<<"the integer is positve number";
        break;
        default:cout<<"its a negative number";
        break;
    }
} 
}
```
> Q15📝
```
#include <iostream>
using namespace std;

int main(){
int num;
cout<<"enter a number here >> ";
cin>>num;

if (num % 10){
    cout<<"it is divisible to 10 completely !";    
} else{
cout<<"its not fuly divide able to 10";
 }
}
```
> Q16📝
```
#include <iostream>
using namespace std;

int main(){
  int lenght , width;

  cout<<"enter the lenght of the rectangle > ";
  cin>>lenght;
  cout<<"enter the widht of the rectangle > ";
  cin>>width;

  if (lenght % 3 == 0 && lenght % 3 == 1){
    cout<<"its a square ";
    if(width % 3 == 0 && width % 3 == 1){
        cout<<"its a square ";
    }
  } else {
    cout<<"its not a square";
  }
}
```
> Q17📝
```
#include <iostream>
using namespace std;

int main(){
    float inverse;
    cout<<"enter a 5 - digit number > ";
    cin>>inverse;
    inverse = 1/inverse;
    cout<<"the inverse of ur number is "<<inverse;
}
```
> Q18📝
```
#include <iostream>
#include <cctype>
using namespace std;
int main(){
    char aplhabet;
    cout<<"enter an alphabet here > ";
    cin>>aplhabet;
    if (islower(aplhabet)){
        cout<<"alphabet is lowercase "<<aplhabet;
    if (isupper(aplhabet)){
     cout<<"alphabet is upper case "<<aplhabet;       
    }
}
}
```
