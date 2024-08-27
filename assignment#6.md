# ASSIGNMENT-6.CPP

### // Write a function to get an array of integers as input parameters and print it.
```
#include <iostream>
using namespace std;

void printarr(int* arr , int size){
for(int i =0 ; i < size; i++){
    cout<<arr[i]<<" ";
}
}
int main(){
    int  n =0;
    int *arr;  //using pointer for dynamic memory allocations 
    cout<<"array size > ";
    cin>>n;
    arr = new int[n]; //used the new function for the dynamic memory allocations iski waja sy humary code mae run time items ki storage bandi ha 
  for(int i =0 ; i < n ; i++){
    cout<<"enter the index "<<i+1<<" > ";
    cin>>arr[i];
  } 
  printarr(arr,n); //passed the arr and size 
return 0;
}


### //2. Write a function to display an array in reverse order.
#include <iostream>
using namespace std;

void reverseArr(int *arr , int size){
for(int i= size-1; i >=0 ; i++){
    cout<<arr[i]<<" ";
}
}

int main(){
 int n =0;
  int *arr;
    cout<<"size of arry > ";
    cin>>n;
    arr = new int[n];
    for(int i=0 ; i < n ; i++){
        cout<<"indexes no."<<i+1<<" > ";
        cin>>arr[i];        
    }  
  cout<<"the array in reverse order is >> ";
  reverseArr(arr , n);
 return 0;
}
```
### //3. Write a function to find the sum of all elements of the array. 
```
#include <iostream>
using namespace std;
int sumofarr(int *arr , int s){
 int sum = 0;
 for(int i =0 ; i < s; i++){
    sum+= arr[i];
 }
  return sum;
}
int main(){
  int n ;
  int *arr; 
    cout<<"the size of array should be > ";
    cin>>n;
    arr = new int[n];
    for(int i = 0 ; i < n ; i++){
        cout <<"enter the value to the array >> ";
        cin>>arr[i];
    }
  int sum = sumofarr(arr , n);
  cout<<"the sum of the array is >> "<<sum;
return 0;
}
```
### //4. Write a function to copy the elements of one array into another array.
```
#include <iostream>
using namespace std;

void copyingFunc(int *arr , int s){
int arr2[s];
cout << "the new array 2 > ";
 for(int i =0 ; i<s;i++){
    arr2[i] = arr[i];
  cout <<arr2[i]<<" ";
 }
}

int main(){
 int n =0;
 int *arr1;
 cout<<"size of array > ";
 cin>>n;
 arr1 = new int[n];
  for(int i=0 ; i<n ; i++){
    cout<<"array 1 index "<<i+1<<" >> ";
    cin>>arr1[i]; 
  } 
 copyingFunc(arr1 , n); 
 return 0;   
}
```
### //5. Write a function to count a total number of duplicate elements in an array.
```
#include <iostream>
using namespace std;

int duplicateFunc(int *arr, int s);

int main() {
 int n; 
  int *arr; 
   cout << "The size of an array should be > ";
    cin >> n;
 arr = new int[n];
  for(int i = 0; i < n; i++){
        cout << "Enter element " << i + 1 << ": ";
        cin >> arr[i];
    }
 int duplications = duplicateFunc(arr, n); 
    cout << "Number of duplications are > " << duplications << endl;
    return 0;
}
int duplicateFunc(int *arr, int s){
 int count = 0;
  for(int i = 0; i < s; i++){
    for(int j = i + 1; j < s; j++){
        if(arr[i] == arr[j]){
          count++;
            break; 
            }
        }
    }
    return count; 
}
```
### //6. Write a function to print all unique elements in an array.
```
#include <iostream>
using namespace std;

void uniqueElements(char element , int s){
 int UNIelemnts[s];
 for(int i = 0 ; i< s ; i++){
  cout<<"enter different number ranging from 30 > 80 input only "<< s <<" amount \n > ";
  cin>> element;
    (char)element;
  UNIelemnts[i] = element;
  cout<<"the elements are "<< UNIelemnts[i] << endl;
  }  
}

int main(){
 int n; 
  char elements;
   cout << "The size of an array should be > ";
    cin >> n; 
   uniqueElements( elements , n);
 return 0;
}
/*#include <iostream>
using namespace std;

void uniqueElements(int *elements, int s) {
    cout << "Enter different numbers ranging from 30 to 80. Input only " << s << " amounts:\n";
    for (int i = 0; i < s; i++) {
        cout << i + 1 << ": ";
        cin >> elements[i];

        // Input validation
        while (elements[i] < 30 || elements[i] > 80) {
            cout << "Please enter a number between 30 and 80: ";
            cin >> elements[i];
        }
    }

    cout << "The unique elements are: ";
    for (int i = 0; i < s; i++) {
        cout << elements[i] << " ";
    }
    cout << endl;
}

int main() {
    int n;
    cout << "The size of an array should be > ";
    cin >> n;

    // Dynamically allocate memory for the elements
    int *elements = new int[n];

    // Call the function to get unique elements
    uniqueElements(elements, n);

    // Free the allocated memory
    delete[] elements;

    return 0;
}*/

```
### // 7. Write a function to merge two arrays of same size sorted in decending order.
```
# include <iostream>
using namespace std;

void mergeFunc(int *arr1 , int *arr2 , int size){
 int arr3[size];
    for(int i = 0 ; i < size ; i++){
        for(int j = 0 ; j <size ; j++){
       arr3[size + size] = arr1[i] + arr2[j];
        }
    }
  cout<<"the merged array is >> \n"<<arr3[size]<<" ";
}

int main(){
 int n =0;
 cout<<"size of array > ";
 cin>>n;
  int *arr1 , *arr2;
 arr1 = new int[n];
 arr2 = new int[n];
 return 0; 
}
```
### //9. Write a function to find the maximum and minimum element in an array.
```
#include <iostream>
using namespace std;
void MaxMiniNumbers(int*arr , int size){
 int maxNum = arr[0];
  int minNum = arr[0]; 
  for(int i = 1 ; i < size ; i++){
    if (arr[i] > maxNum){
      maxNum = arr[i];
    }
    if (arr[i] < minNum){
        minNum = arr[i];
   }
     
  }    
  cout << "maximum number >> "<<maxNum <<endl;
  cout << "minimum number >> "<<minNum <<endl; 
}

int main(){
 int n = 0;
  int *arr;
 cout<<"size of array > ";
 cin>>n;
 arr = new int[n];
  cout << "enter " << n << " elements > " << endl;
    for (int i = 0; i < n; i++){
        cout << "element " << i + 1 << ": ";
        cin >> arr[i];
    }
 MaxMiniNumbers(arr , n);
 return 0;
}
```
### //10. Write a function to separate odd and even integers in separate arrays.
```
#include <iostream>
using namespace std;
void OddEvenNum(int *arr , int size){
 int odd[size];
 int even[size];
 int evencount = 0 ;
 int oddcount =0;
 for(int i=0 ; i < size ; i++){
    if(arr[i]%2 == 0){
     even[evencount] = arr[i];
     evencount++;
    }
    if(arr[i]%2 != 0){
    odd[oddcount] = arr[i];
    oddcount++;
    }
 }
  for(int i = 0; i < evencount && i < oddcount ; i++){
    cout<<"even numbers >> "<<even[i]<< endl;
    cout<<"odd numbers >> "<<odd[i]<< endl;
  }
}
int main(){
 int n = 0;
  int *arr;
 cout<<"size of array > ";
 cin>>n;
 arr = new int[n];
  cout << "enter " << n << " elements > " << endl;
    for (int i = 0; i < n; i++){
        cout << "element " << i + 1 << ": ";
        cin >> arr[i];
    }
 OddEvenNum(arr , n);
 return 0;
}
```
### //11. Write a function to sort elements of array in ascending order.
```
#include <iostream>
using namespace std;
void AsendingArr(int *arr , int size ){
  for (int i = 0; i < size - 1; i++){
        for (int j = 0; j < size - i - 1; j++){
            if (arr[j] > arr[j + 1]){ 
                int temp = arr[j];
                arr[j] = arr[j + 1];
                arr[j + 1] = temp;
            }
        }
    }
    cout << "Sorted array in ascending order >> ";
    for (int i = 0; i < size; i++){
        cout << arr[i] << " ";
    }
    cout << endl;
}

int main(){
int n = 0;
  int *arr;
 cout<<"size of array > ";
 cin>>n;
 arr = new int[n];
  cout << "enter " << n << " elements > " << endl;
    for (int i = 0; i < n; i++){
        cout << "element " << i + 1 << ": ";
        cin >> arr[i];
    }
  AsendingArr(arr , n);
 return 0;
}
```
### //12. Write a function to sort elements of the array in descending order.
```
#include <iostream>
using namespace std;
void DsendingArr(int *arr , int size ){
  for (int i = 0; i < size - 1; i++){
    for (int j = 0; j < size - i - 1; j++){
      if (arr[j] < arr[j + 1]){ 
        int temp = arr[j];
         arr[j] = arr[j + 1];
            arr[j + 1] = temp;
      }
    }
  }  
  cout << "Sorted array in descending order: ";
    for (int i = 0; i < size; i++){
      cout << arr[i] << " ";
    }
  cout << endl;
}

int main(){
int n = 0;
  int *arr;
 cout<<"size of array > ";
 cin>>n;
 arr = new int[n];
  cout << "enter " << n << " elements > " << endl;
    for (int i = 0; i < n; i++){
        cout << "element " << i + 1 << ": ";
        cin >> arr[i];
    }
  DsendingArr(arr , n);
 return 0;
}
```
### // 13. Write a function to insert New value in the array (sorted list )
```
#include <iostream>
using namespace std;

void InsertionFunc(int *arr , int size){
 int newValue;
  cout << "enter the new value to be inserted > ";
  cin >> newValue;
  int i;
    for (i = size - 1; (i >= 0 && arr[i] > newValue); i--){
      arr[i + 1] = arr[i]; 
    }
  arr[i + 1] = newValue;
  cout << "updated sorted array > ";
    for (int j = 0; j <= size; j++){
        cout << arr[j] << " "; 
    }
  cout << endl;
}
int main(){
int n = 0;
  int *arr;
 cout<<"size of array > ";
 cin>>n;
 arr = new int[n+1];
  cout << "enter " << n << " elements > " << endl;
    for (int i = 0; i < n; i++){
        cout << "element " << i + 1 << ": ";
        cin >> arr[i];
    }
   InsertionFunc(arr , n); 
return 0;
}
```
### //14. Write a function to insert New value in the array (unsorted list ).
```
#include <iostream>
using namespace std;

void InsertionFunc(int *arr , int size){
 int newValue;
  cout << "enter the new value to be inserted > ";
  cin >> newValue;
  arr[size] = newValue;
  cout << "Updated array > ";
    for (int i = 0; i <= size; i++){
      cout << arr[i] << " "; 
    }
  cout << endl;
}
int main(){
int n = 0;
  int *arr;
 cout<<"size of array > ";
 cin>>n;
 arr = new int[n+1];
  cout << "enter " << n << " elements > " << endl;
    for (int i = 0; i < n; i++){
        cout << "element " << i + 1 << ": ";
        cin >> arr[i];
    }
   InsertionFunc(arr , n); 
return 0;
}
```
### //15. Write a program in C to delete an element at desired position from an array
```
#include <iostream>
using namespace std;

void DelFunc(int *arr , int size){
 int position;
   cout << "Enter the position of the element to be deleted > ";
    cin >> position;
  for (int i = position - 1; i < size - 1; i++) {
    arr[i] = arr[i + 1];
  }
    cout << "Updated array > "; 
  for (int i = 0; i < size - 1; i++){
    cout << arr[i] << " ";
  }
  cout << endl;
}
int main(){
    int n = 0;
  int *arr;
 cout<<"size of array > ";
 cin>>n;
 arr = new int[n];
  cout << "enter " << n << " elements" << endl;
    for (int i = 0; i < n; i++){
        cout << "element " << i + 1 << ": ";
        cin >> arr[i];
    }
  DelFunc(arr , n);
 return 0;
}
```
### //16. Write a function to find the second largest element in an array. 
```
#include <iostream>
using namespace std;
void SecLargestElement(int *arr , int size){
 int largest = arr[0];
  int secondLargest = -1; 
  for (int i = 1; i < size; i++){
    if (arr[i] > largest){
      secondLargest = largest;
        largest = arr[i]; 
    } 
     else if (arr[i] > secondLargest && arr[i] < largest){
        secondLargest = arr[i]; 
      }
  }
  if (secondLargest == -1){
    cout << "There is no second largest element." << endl;
  } 
  else{
    cout << "The second largest element is > " << secondLargest << endl;
  }
}
int main(){
 int n = 0;
  int *arr;
 cout<<"size of array > ";
 cin>>n;
 arr = new int[n];
  cout << "enter " << n << " elements" << endl;
    for (int i = 0; i < n; i++){
        cout << "element " << i + 1 << ": ";
        cin >> arr[i];
    }
    SecLargestElement(arr , n);
 return 0;   
}
```
### //18. Write a function to get input from user for a 2D array of size 3x3 and print the matrix.
```
#include <iostream>
using namespace std;
void Arrayfunction(){
    int FuncArr[3][3];
     cout<<"enter the elements to the arr1 > \n";
  for(int i =0 ; i<3 ; i++){
    for(int j =0 ; j<3 ; j++){
     cout << "element ["<<i<<"]"<<"["<<j<<"]"<<" >> ";
      cin>>FuncArr[i][j];
    }
  }
  cout<<"3x3 matrix\n";
  for(int i = 0 ; i<3 ; i++){
      for(int j = 0 ; j<3 ; j++){
          cout << FuncArr[i][j] << " ";
  }
    cout<<endl;
  }
}
int main(){
 Arrayfunction();
 return 0;
}
```
### //19. Write a function to add two Matrices of same size. //20. Write a function to subtract two Matrices //21. Write a function to multiply two square Matrices.
```
#include <iostream>
using namespace std; 
void SumFuc(int (*arr)[3] , int rows){
  cout<<"make new array in order to add the two matrix\n";
   int arr2[3][rows];
for(int i=0 ;i<3;i++){
  for(int j=0; j<rows ;j++){
    cout<<"element of array2{"<<i<<"}"<<"{"<<j<<"}"<<": ";
    cin >> arr2[i][j];
  }
} 
int sum[3][rows];
for(int i =0 ; i<3 ; i++){
  for(int j =0 ; j<rows ; j++){
    sum[i][j] = arr[i][j] + arr2[i][j];
  }
}
 for(int i =0 ; i < 3 ; i++){
  for(int j =0 ; j<rows ;j++){
    cout<<sum[i][j]<<" ";
  }
  cout<<endl;
 }
}
void MinusFuc(int (*arr)[3] , int rows){
  cout<<"make new array in order to subtract the two matrix\n";
   int arr2[3][rows];
for(int i=0 ;i<3;i++){
  for(int j=0; j<rows ;j++){
    cout<<"element of array2{"<<i<<"}"<<"{"<<j<<"}"<<": ";
    cin >> arr2[i][j];
  }
} 
int minus[3][rows];
for(int i =0 ; i<3 ; i++){
  for(int j =0 ; j<rows ; j++){
    minus[i][j] = arr[i][j] - arr2[i][j];
  }
}
for(int i =0 ; i < 3 ; i++){
  for(int j =0 ; j<rows ;j++){
    cout<<minus[i][j]<<" ";
  }
  cout<<endl;
 }
}
void MultiFunc(int (*arr)[3] , int rows){
  cout<<"make new array in order to multiply the two matrix\n";
   int arr2[3][rows];
for(int i=0 ;i<3;i++){
  for(int j=0; j<rows ;j++){
    cout<<"element of array2{"<<i<<"}"<<"{"<<j<<"}"<<": ";
    cin >> arr2[i][j];
  }
} 
int multi[3][rows];
for(int i =0 ; i<3 ; i++){
  for(int j =0 ; j<rows ; j++){
    multi[i][j] = arr[i][j] * arr2[i][j];
  }
}
 for(int i =0 ; i < 3 ; i++){
  for(int j =0 ; j<rows ;j++){
    cout<<multi[i][j]<<" ";
  }
  cout<<endl;
 }
}
int main(){
int arr[3][3];
for(int i=0 ;i<3;i++){
  for(int j=0; j<3 ;j++){
    cout<<"element of array1{"<<i<<"}"<<"{"<<j<<"}"<<": ";
    cin >> arr[i][j];
  }
}
 int options;
 cout<<"press 1 for add\npress 2 for minus\npress 3 for multiplication\n";
 cin>>options;
 switch(options){
  case 1 : SumFuc(arr, 3);
  break;
  case 2 : MinusFuc(arr , 3);
  break;
  case 3 : MultiFunc(arr , 3);
  break;
  default : "Error <invalid>-<option>";
  break;
 }
 return 0; 
}
```
### //22. Write a function to find transpose of a given matrix.
```
#include <iostream>
 using namespace std;

void TransposeFunc(int arr[3][3]){
 int tranpose[3][3];
  for(int i=0 ; i<3 ; i++){
   for(int j=0 ; j<3 ; j++){
    tranpose[j][i] = arr[i][j];
  }
 }
 cout<<"the transpose matix is\n";
  for(int i=0 ; i<3 ; i++){
   for(int j=0 ; j<3 ; j++){
    cout<<tranpose[i][j]<<" "; 
  }
 cout<< endl;
 }
}
int main(){
 int arr[3][3];
  for(int i =0 ; i<3 ; i++){
   for(int j=0 ; j<3 ; j++){
    cout<<"element ["<<i<<"]["<<j<<"]"<<" : ";
     cin>>arr[i][j];
  }
 }
 cout<<"orignal matrix\n";
  for(int i =0 ; i<3 ; i++){
  for(int j=0 ; j<3 ; j++){
    cout<<arr[i][j]<<" ";
  }
  cout<<endl;
 }
 TransposeFunc(arr);
return 0;
}
```
### //24. Write a function to find sum of left diagonals of a matrix
```
#include <iostream>
using namespace std;
void SumDiagonals(int arr[3][3]){
int sum = 0;
  for (int i = 0; i < 3; i++){
    sum += arr[i][i]; 
    }
  cout << "left diagonal elements are >\n";
    for (int i = 0; i < 3; i++){
      cout << arr[i][i] << " "; 
    }
  cout << endl;

  cout << "sum of left diagonal elements > " << sum << endl;
}
int main(){
  int arr[3][3];
  for(int i =0 ; i<3 ; i++){
   for(int j=0 ; j<3 ; j++){
    cout<<"element ["<<i<<"]["<<j<<"]"<<" : ";
     cin>>arr[i][j];
  }
 }
 cout<<"the martix u typed >>\n";
  for(int i =0 ; i<3 ; i++){
   for(int j=0 ; j<3 ; j++){
     cout<<arr[i][j]<<" ";
  }
    cout<<endl;
  }
 SumDiagonals(arr);
 return 0;
}
```
### //25. Write a program in C to find sum of rows an columns of a Matrix
```
#include <iostream>
using namespace std;
void SumOfRowsCol(int arr[2][2]){
 int SumRow[2] ={0};
 int SumCol[2] ={0};
  for(int i =0 ; i<2;i++){
    for(int j = 0 ; j<2;j++){
      SumRow[i] += arr[i][j];
      SumCol[j] += arr[i][j];
    }
  }
  for(int i =0 ; i <2 ; i++){
    cout<<"Sum of Rows > "<<i<<" : "<<SumRow[i]<< endl;
  }
  for(int j =0 ; j <2 ; j++){
    cout<<"Sum of col > "<<j<<" : "<<SumCol[j]<< endl;
  }
}
int main(){
  int arr[2][2];
  for(int i =0 ; i<2 ; i++){
    for(int j =0 ; j<2 ; j++){
      cout<<"elements ["<<i<<"]["<<j<<"]"<<" : ";
      cin>>arr[i][j];
    }
  }
  cout<<"the matrix is > \n";
 for(int i = 0 ; i<2; i++){
    for(int j =0 ; j<2;j++){
      cout << arr[i][j]<<" ";
    }
  cout<<endl;
}
 SumOfRowsCol(arr);
 return 0;
}
```
# /*26. Write a program in C to print or display the lower triangular of a given matrix. 27. Write a program in C to print or display upper triangular matrix*/
```
#include <iostream>
using namespace std;
void UpperTriangel(int arr[3][3]){
cout << "\nupper triangular matrix > \n";
  for (int i = 0; i < 3; i++){
    for (int j = 0; j < 3; j++){
      if (j >= i){
       cout << arr[i][j] << " ";
      } else{
          cout << "0 ";
        }
    }
  cout << endl;
  }
}
void LowerTriangel(int arr[3][3]){
 cout << "\nlower triangular matrix > \n";
  for (int i = 0; i < 3; i++){
    for (int j = 0; j < 3; j++){
      if (j <= i){
       cout << arr[i][j] << " ";
      } else {
          cout << "0 ";
        }
    }
  cout << endl;
  }
}
int main(){
 int arr[3][3];
  for(int i =0 ; i<3 ; i++){
   for(int j =0 ; j<3 ; j++){
    cout<<"elements ["<<i<<"]["<<j<<"]"<<" : ";
     cin>>arr[i][j];
    }
  }
  int options;
  cout<<"enter options\npress 1 for upper triangel\npress 2 for lower triangel\n>>";
  cin>>options;
 switch(options){
  case 1: UpperTriangel(arr);
  break;
  case 2 : LowerTriangel(arr);
  break;
  default: cout <<"<INVAILD OPTIONS>";
  break; 
 }
 return 0;
}
```
# //28. Write a program in C to calculate determinant of a 3 x 3 matrix.
```
#include <iostream>
using namespace std;

void DeterminantFunc(int arr[2][2]){
int determinant = arr[0][0] * arr[1][1] - arr[0][1] * arr[1][0];
  cout << "The determinant of the matrix is > " << determinant << endl;
}
int main(){
 int arr[2][2];
  cout << "Enter the elements of the 2x2 matrix >\n";
    for (int i = 0; i < 2; i++){
      for (int j = 0; j < 2; j++){
      cout << "Enter element a" << i + 1 << j + 1 << " > ";
        cin >> arr[i][j];
    }
  }
 return 0;
}
```
