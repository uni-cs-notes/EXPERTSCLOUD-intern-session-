> Assignment # 1 ✅
```
 #include <iostream>
using namespace std;

int main(){
    int n1 , n2;
    cout<<"enter integers >> ";
    cin>>n1>>n2;
    int sum = n1 + n2;
    cout<<"sum >> " << sum;
}

```
> Q1 ✏️
```
#include <iostream>
using namespace std;


int main(){
   int x = 5 ;
   int y = 10 ;
cout << "before Swapping \n >> x = " << x << "\n >>y = " <<y;
int z = x;
x = y;
y = z;
cout <<"after Swapping \n >> x = " << x << "\n >>y = "<<y;
}
```
> Q2 ✏️
```


#include <iostream>
using namespace std;


int main(){
   float radius = 0;
   cout<<"enter the radius  >> ";
   cin>>radius;
 float vol = 4*3.1415*radius*radius*radius;
 cout<<"volume of shpere >> "<<vol;


}
```
> Q3 ✏️
```
#include <iostream>
using namespace std;


int main(){
   float side = 0;
   cout<<"enter the side  >> ";
   cin>>side;
 float vol = side*side*side;
 cout<<"volume of cube >> "<<vol;
}
```
> Q4 ✏️
```
#include <iostream>
using namespace std;


int main(){
   cout<<"\t\t area ";
   int lenght = 0;
   cout<<"lenght  >> ";
   cin>>lenght;
   int width = 0;
   cout<<"width >> ";
   cin>>width;
 int area = lenght * width;
 cout<<"AREA >> "<< area;
}
```
> Q5 ✏️
```
#include <iostream>
using namespace std;


int main(){
   cout<<"\t\t area of circle ";
   float radius = 0 ;
   cout<<"enter radius of circle >> ";
   cin>>radius;
   float area = 3.1415*radius*radius;
   cout<<"area of circle > "<<area;
   float circum = 2 \ 3.1415 * radius;
   cout<<"circumference of circle > "<<circum;
}
```
> Q6 ✏️
 ```
#include <iostream>
using namespace std;


int main(){
   int fahrenheit , celsius;
   cout<<"enter ur temp in fahrenheit > ";
   cin>>fahrenheit;
   celsius = ((fahrenheit * 5)-(5 * 32))/9;
   cout<<"ur temp in celsius >> "<<celsius;
}
```
> Q7 ✏️
```

#include <iostream>
using namespace std;


int main(){
   int ang1 , ang2 , ang3 ;
   cout<<"angel 1 > ";
   cin>>ang1;
   cout<<"angel 2 > ";
   cin>>ang2;
   ang3 = 180 - (ang1 + ang2);
   cout<<"third angel will be > "<< ang3;
}
```
> Q8 ✏️
```

#include <iostream>
using namespace std;


int main(){
   int km = 0 ;
   cout<<"enter distance covered in KM > ";
   cin>>km;
   float mile = km * 0.6213712 ;
   cout<< "KM covered in miles are > "<< mile;
}
```
> Q9 ✏️
```

int main(){
   float dividend , divisor;
   cout << "enter ur divisor (the number u will divide with) > ";
   cin>>divisor;
   cout<<"enter ur dividend (the number being divided) > ";
   cin>>dividend;
   float quotient = dividend /divisor  ;
   float remainder = dividend % divisor ;  >>(error)
cout<<"the quotient will be > "<<quotient<<"\n";
cout<< "the remainder will be > "<<remainder<<"\n";
}
```
> Q10 ✏️
```

#include <iostream>
#include <cmath>
using namespace std;


int main(){
   float dividend , divisor;
   cout << "enter ur divisor (the number u will divide with) > ";
   cin>>divisor;
   cout<<"enter ur dividend (the number being divided) > ";
   cin>>dividend;
   float quotient = dividend /divisor  ;
   float remainder = fmod (dividend,divisor) ; // was giving error lately! (bug fixed)
cout<<"the quotient will be > "<<quotient<<"\n";
cout<< "the remainder will be > "<<remainder<<"\n";
}
```
>  Q11 ✏️


```

#include <iostream>
using namespace std;


int main(){
   int num[4];
  
   for(int i=0;i<4;i++){
       cin>>num[i];
   }
  int avg = (num[0]+num[1]+num[2]+num[3]) /4;
 cout<<"total avg is > "<<avg;
}
```
> Q12 ✏️
```

#include <iostream>
using namespace std;


int main(){


 //implicit type casting
 int v1 = 9;
 float v2 = 2.25;
// now we will type cast our variables
int n1 = v2;
float n2 = v1;


//explicit typecasting


int x = 5;
float y = 2.554;
// now change the value through the explicit type casting method
int x1 = (int)y;
float y1 = (float)x;

}

```
>  Q13 ✏️
```

#include <iostream>
using namespace std;


int main(){
int n ;
cout<<"enter ur number here > ";
cin>>n;
for(int i = 1 ; i < 10 ;i++){
   cout<<" "<<n<<" x "<<i<<" = " << n*i << endl ;
}
return 0;
}
```


