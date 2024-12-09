### 1. Write a program in C to store elements in an array and print it.*/
```
#include <iostream>
using namespace std;

int main(){
    int num[5];
    cout<<"enter 5 number >> \n";
    for( int i = 0 ; i < 5 ; i++){
        cin>>num[i];
    } 
    for (int i = 0 ; i < 5 ; i++){
        cout<<"the numbers positions are "<<i<<" >> "<<num[i]<<endl;
    }
  return 0;
}
```
### 2. Write a program in C to read n number of values in an array and display it in reverse order.*/
```
#include <iostream>
using namespace std;

int main(){
    int n =0;
    cout<<"enter the size of array u want  > ";
    cin>>n;
    int num[n];
    for(int i = 0 ; i < n ; i++){
         cout<<"enter the values for the arrays  >> ";
         cin>>num[i];
    } 

    for(int i= n-1 ; i >=0 ; i--){
        cout<<"the array in reverse order is > "<< num[i]<<endl;
    }
 return 0;
}
```
### 3. Write a program in C to find the sum of all elements of the array. */
```
#include <iostream>
using namespace std;

int main(){
    int n ; 
    cout<<"the size of array should be > ";
    cin>>n;
    int num[n];
    int sum =0 ;
    for(int i = 0 ; i < n ; i++){
        cout <<"enter the value to the array >> ";
        cin>>num[i];
        sum += num[i];
    }
    cout<<"the sum is > "<< sum << endl;
 return 0;
}
```
### 4. Write a program in C to copy the elements of one array into another array.*/
```
#include <iostream>
using namespace std;
int main(){
  int n ; 
    cout<<"the size of an array should be > ";
    cin>>n;
    int num[n];
    int num2[n];
    for(int i = 0 ; i < n ; i++){
    cout<<"array 1 >> ";
    cin>>num[i];
    num2[i] = num[i];     
    }
    for(int i = 0 ;i < n ; i++ ){
        cout<<"array 2 >> "<<num2[i]<<endl;
     }
    
 return 0;
}   
```
### 5. Write a program in C to count a total number of duplicate elements in an array.*/
```
#include <iostream>
using namespace std;
int main(){
    int n ; 
    cout<<"the size of an array should be > ";
    cin>>n;
    int num[n];
    int count =0;
    for(int i = 0 ; i < n ; i++){
    cout<<"array  >> ";
    cin>>num[i];
    }
     for(int i = 0 ; i < n ; i++){
        for(int j = i + 1 ; j < n ; j++){
          if (num[i] == num[j]){
            count++;
          }
        }
    } 
     cout <<"number of duplications > "<< count << endl;
 return 0;
}
```
### 6. Write a program in C to print all unique elements in an array. */
```
#include <iostream>
using namespace std;

 int main(){
 int n =0;
 cout<<"enter the size of array > ";
 cin>>n;
  char Unielements[n];
  int elements =0 ;
  for(int i = 0 ; i< n ; i++){
  cout<<"enter different number ranging from 30 > 80 input only "<< n-1 <<" amount \n > ";
  cin>> elements;
    (char)elements; //typecasting from int to char
   Unielements[n] = elements;
    cout<<"the elemnts are > "<< Unielements[n] << endl;
  }
  return 0;
}
```
### 7. Write a program in C to merge two arrays of same size sorted in decending order.*/
```
#include <iostream>
using namespace std;
int main(){
  int arr1[4] = {5,7,9,6};
  int arr2[4] = {4,8,10,1};
  int arr3[8];
  for(int i = 0 ; i < 4 ; i++){
    for(int j = 0 ; j < 4 ; j++){
     arr3[8] = arr1[i] + arr2[j] ;
    }
  } 

}
```
### 9. Write a program in C to find the maximum and minimum element in an array.*/
```
#include <iostream>
using namespace std;

int main(){
  int n =0;
  cout<<"enter the size of an array > ";
  cin>>n;
  int arr[n];
  for(int i = 0 ; i < n ; i++){
    cout <<i+1<<" >> ";
    cin>>arr[i];
  }
  int maxNum = arr[0];
  int minNum = arr[0]; //use the 1st elemnt as starting point for both max and mini numbers 
  for(int i = 1 ; i < n ; i++){
    if (arr[i] > maxNum){
      maxNum = arr[i];
    }
    if (arr[i] < minNum){
        minNum = arr[i];
   }
     
  }    
  cout << "maximum number >> "<<maxNum <<endl;
  cout << "minimum number >> "<<minNum <<endl; 
 return 0;
}
```
### 10. Write a program in C to separate odd and even integers in separate arrays.*/
```
#include <iostream>
using namespace std;

int main(){
  int arr[8] = {5,9,2,7,65,99,32,1};
  int even[8];
  int odd[8];
  int evenCount , oddCount;

  for(int i = 0 ; i < 8;i++){
    if(arr[i]%2 == 0){
      even[evenCount] = arr[i]; 
      evenCount++;
    }
    if(arr[i]%2 != 0 ){
     odd[oddCount] = arr[i];
     oddCount++;
    }
  }
  for(int i = 0 ; i < evenCount ; i++){
  cout << "even numbers >> "<< even[i] << endl;
  } 
  for(int i = 0 ; i < oddCount ; i++){
  cout << "odd numbers >> "<< odd[i] << endl;
  }
return 0;
}
```
### 11. Write a program in C to sort elements of array in ascending order.
### 12. Write a program in C to sort elements of the array in descending order.*/
```
#include <iostream>
using namespace std;

int main(){
  int n;
  cout << "Enter the size of the array: ";
  cin >> n;
  int arr[n]; 
  cout << "Enter the array elements:\n";
   for (int i = 0; i < n; i++){
      cin >> arr[i];
    }

    for (int i = 0; i < n - 1; i++){
        for (int j = 0; j < n - i - 1; j++){
            if (arr[j] < arr[j + 1]){ 
                int temp = arr[j];
                arr[j] = arr[j + 1];
                arr[j + 1] = temp;
            }
        }
    }

    
  cout << "Sorted array in descending order: ";
    for (int i = 0; i < n; i++){
      cout << arr[i] << " ";
    }
  cout << endl;

  return 0;
}
```
### // asending order
```
#include <iostream>
using namespace std;

int main(){
    int n;
    cout << "Enter the size of the array > ";
    cin >>n;
    int arr[n]; 
    cout << "Enter the array elements\n";
    for (int i = 0; i < n; i++) {
        cout<<">> ";
        cin >> arr[i];
    }
    for (int i = 0; i < n - 1; i++){
        for (int j = 0; j < n - i - 1; j++){
            if (arr[j] > arr[j + 1]){ 
                int temp = arr[j];
                arr[j] = arr[j + 1];
                arr[j + 1] = temp;
            }
        }
    }
    cout << "Sorted array in ascending order >> ";
    for (int i = 0; i < n; i++){
        cout << arr[i] << " ";
    }
    cout << endl;

    return 0;
}
```
### 13. Write a program in C to insert New value in the array (sorted list )*/
### 1. Write a program in C to store elements in an array and print it.*/
```
#include <iostream>
using namespace std;

int main(){
    int num[5];
    cout<<"enter 5 number >> \n";
    for( int i = 0 ; i < 5 ; i++){
        cin>>num[i];
    } 
    for (int i = 0 ; i < 5 ; i++){
        cout<<"the numbers positions are "<<i<<" >> "<<num[i]<<endl;
    }
  return 0;
}

/*2. Write a program in C to read n number of values in an array and display it in reverse order.*/

#include <iostream>
using namespace std;

int main(){
    int n =0;
    cout<<"enter the size of array u want  > ";
    cin>>n;
    int num[n];
    for(int i = 0 ; i < n ; i++){
         cout<<"enter the values for the arrays  >> ";
         cin>>num[i];
    } 

    for(int i= n-1 ; i >=0 ; i--){
        cout<<"the array in reverse order is > "<< num[i]<<endl;
    }
 return 0;
}
```
### 3. Write a program in C to find the sum of all elements of the array. */
```
#include <iostream>
using namespace std;

int main(){
    int n ; 
    cout<<"the size of array should be > ";
    cin>>n;
    int num[n];
    int sum =0 ;
    for(int i = 0 ; i < n ; i++){
        cout <<"enter the value to the array >> ";
        cin>>num[i];
        sum += num[i];
    }
    cout<<"the sum is > "<< sum << endl;
 return 0;
}
```
### 4. Write a program in C to copy the elements of one array into another array.*/
```
#include <iostream>
using namespace std;
int main(){
  int n ; 
    cout<<"the size of an array should be > ";
    cin>>n;
    int num[n];
    int num2[n];
    for(int i = 0 ; i < n ; i++){
    cout<<"array 1 >> ";
    cin>>num[i];
    num2[i] = num[i];     
    }
    for(int i = 0 ;i < n ; i++ ){
        cout<<"array 2 >> "<<num2[i]<<endl;
     }
    
 return 0;
}   
```
### 5. Write a program in C to count a total number of duplicate elements in an array.*/
```
#include <iostream>
using namespace std;
int main(){
    int n ; 
    cout<<"the size of an array should be > ";
    cin>>n;
    int num[n];
    int count =0;
    for(int i = 0 ; i < n ; i++){
    cout<<"array  >> ";
    cin>>num[i];
    }
     for(int i = 0 ; i < n ; i++){
        for(int j = i + 1 ; j < n ; j++){
          if (num[i] == num[j]){
            count++;
          }
        }
    } 
     cout <<"number of duplications > "<< count << endl;
 return 0;
}
```
### 6. Write a program in C to print all unique elements in an array. */
```
#include <iostream>
using namespace std;

 int main(){
 int n =0;
 cout<<"enter the size of array > ";
 cin>>n;
  char Unielements[n];
  int elements =0 ;
  for(int i = 0 ; i< n ; i++){
  cout<<"enter different number ranging from 30 > 80 input only "<< n-1 <<" amount \n > ";
  cin>> elements;
    (char)elements; //typecasting from int to char
   Unielements[n] = elements;
    cout<<"the elemnts are > "<< Unielements[n] << endl;
  }
  return 0;
}
```
### 7. Write a program in C to merge two arrays of same size sorted in decending order.*/
```
#include <iostream>
using namespace std;
int main(){
  int arr1[4] = {5,7,9,6};
  int arr2[4] = {4,8,10,1};
  int arr3[8];
  for(int i = 0 ; i < 4 ; i++){
    for(int j = 0 ; j < 4 ; j++){
     arr3[8] = arr1[i] + arr2[j] ;
    }
  } 
return 0;
}
```
### 9. Write a program in C to find the maximum and minimum element in an array.*/
```
#include <iostream>
using namespace std;

int main(){
  int n =0;
  cout<<"enter the size of an array > ";
  cin>>n;
  int arr[n];
  for(int i = 0 ; i < n ; i++){
    cout <<i+1<<" >> ";
    cin>>arr[i];
  }
  int maxNum = arr[0];
  int minNum = arr[0]; //use the 1st elemnt as starting point for both max and mini numbers 
  for(int i = 1 ; i < n ; i++){
    if (arr[i] > maxNum){
      maxNum = arr[i];
    }
    if (arr[i] < minNum){
        minNum = arr[i];
   }
     
  }    
  cout << "maximum number >> "<<maxNum <<endl;
  cout << "minimum number >> "<<minNum <<endl; 
 return 0;
}
```
### 10. Write a program in C to separate odd and even integers in separate arrays.*/
```
#include <iostream>
using namespace std;

int main(){
  int arr[8] = {5,9,2,7,65,99,32,1};
  int even[8];
  int odd[8];
  int evenCount , oddCount;

  for(int i = 0 ; i < 8;i++){
    if(arr[i]%2 == 0){
      even[evenCount] = arr[i]; 
      evenCount++;
    }
    if(arr[i]%2 != 0 ){
     odd[oddCount] = arr[i];
     oddCount++;
    }
  }
  for(int i = 0 ; i < evenCount ; i++){
  cout << "even numbers >> "<< even[i] << endl;
  } 
  for(int i = 0 ; i < oddCount ; i++){
  cout << "odd numbers >> "<< odd[i] << endl;
  }
return 0;
}
```
### 11. Write a program in C to sort elements of array in ascending order.
### 12. Write a program in C to sort elements of the array in descending order.*/
```
#include <iostream>
  using namespace std;

int main(){
  int n;
  cout << "Enter the size of the array: ";
  cin >> n;
  int arr[n]; 
  cout << "Enter the array elements:\n";
   for (int i = 0; i < n; i++){
      cin >> arr[i];
    }

    for (int i = 0; i < n - 1; i++){
        for (int j = 0; j < n - i - 1; j++){
            if (arr[j] < arr[j + 1]){ 
                int temp = arr[j];
                arr[j] = arr[j + 1];
                arr[j + 1] = temp;
            }
        }
    }

    
  cout << "Sorted array in descending order: ";
    for (int i = 0; i < n; i++){
      cout << arr[i] << " ";
    }
  cout << endl;

  return 0;
}
```
### // asending order
```
#include <iostream>
using namespace std;

int main(){
    int n;
    cout << "Enter the size of the array > ";
    cin >>n;
    int arr[n]; 
    cout << "Enter the array elements\n";
    for (int i = 0; i < n; i++) {
        cout<<">> ";
        cin >> arr[i];
    }
    for (int i = 0; i < n - 1; i++){
        for (int j = 0; j < n - i - 1; j++){
            if (arr[j] > arr[j + 1]){ 
                int temp = arr[j];
                arr[j] = arr[j + 1];
                arr[j + 1] = temp;
            }
        }
    }
    cout << "Sorted array in ascending order >> ";
    for (int i = 0; i < n; i++){
        cout << arr[i] << " ";
    }
    cout << endl;

    return 0;
}
```
### 13. Write a program in C to insert New value in the array (sorted list )*/
```
#include <iostream>
using namespace std;

int main() {
  int n;
  cout << "Enter the size of the array > ";
  cin >> n;

  int arr[n + 1]; 
  cout << "Enter the sorted array elements > \n";
    for (int i = 0; i < n; i++){
      cin >> arr[i];
    }
  int newValue;
  cout << "Enter the new value to be inserted > ";
  cin >> newValue;
  int i;
    for (i = n - 1; (i >= 0 && arr[i] > newValue); i--) {
      arr[i + 1] = arr[i]; 
    }
  arr[i + 1] = newValue;
  cout << "Updated sorted array > ";
    for (int j = 0; j <= n; j++){
        cout << arr[j] << " "; 
    }
  cout << endl;

  return 0;
}
```
### 14. Write a program in C to insert New value in the array (unsorted list ).*/
```
#include <iostream>
using namespace std;

int main() {
  int n;
  cout << "Enter the size of the array > ";
  cin >> n;

  int arr[n + 1];
  cout << "Enter the unsorted array elements \n";
    for (int i = 0; i < n; i++) {
      cin >> arr[i];
    }
  int newValue;
  cout << "Enter the new value to be inserted > ";
  cin >> newValue;

  arr[n] = newValue;

  cout << "Updated array > ";
    for (int i = 0; i <= n; i++){
      cout << arr[i] << " "; 
    }
  cout << endl;

  return 0;
}
```
### 15. Write a program in C to delete an element at desired position from an array.*/
```
#include <iostream>
using namespace std;

int main(){
  int n;
  cout << "Enter the size of the array > ";
  cin >> n;

  int arr[n];
    
  for (int i = 0; i < n; i++){
    cout << "Enter the array elements at position "<<i+1<<" >> ";
      cin >> arr[i];
  }
  int position;
  cout << "Enter the position of the element to be deleted > ";
  cin >> position;
  for (int i = position - 1; i < n - 1; i++) {
    arr[i] = arr[i + 1];
  }
  
  cout << "Updated array > ";
  
  for (int i = 0; i < n - 1; i++){
    cout << arr[i] << " ";
  }
  cout << endl;

  return 0;
}
```
### 16. Write a program in C to find the second largest element in an array. 
### 17. Write a program in C to find the second smallest element in an array.*/
```
#include <iostream>
using namespace std;

int main() {
  int n;
  cout << "Enter the size of the array > ";
  cin >> n;
  int arr[n];

  for (int i = 0; i < n; i++){
    cout<<"Enter the array element > "<<i+1<<" > "; 
      cin >> arr[i];
  }

  int largest = arr[0];
  int secondLargest = -1; 
  for (int i = 1; i < n; i++){
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

  return 0;
}
```
### //second smallest value  
```
#include <iostream>
using namespace std;

int main(){
  int n;
  cout << "Enter the size of the array > ";
  cin >> n;
  int arr[n];
  for (int i = 0; i < n; i++) {
  cout<<"Enter the array elements "<<i+1<<" > ";
    cin >> arr[i];
  }

  int smallest = arr[0];
  int secondSmallest = -1; 

  for (int i = 1; i < n; i++){
    if (arr[i] < smallest){
      secondSmallest = smallest; 
        smallest = arr[i]; 
    } 
    else if (arr[i] < secondSmallest && arr[i] > smallest){
      secondSmallest = arr[i]; 
    }
  }

  if (secondSmallest == -1){
     cout << "There is no second smallest element." << endl;
  } else{
    cout << "The second smallest element is: " << secondSmallest << endl;
  }
  return 0;
}
```
### 18. Write a program in C for a 2D array of size 3x3 and print the matrix.
### 19. Write a program in C for addition of two Matrices of same size.
### 20. Write a program in C for subtraction of two Matrices
### 21. Write a program in C for multiplication of two square Matrices.*/
```
#include <iostream>
using namespace std;

int main(){
 int arr1[3][3] , arr2[3][3] , sum[3][3] , minus[3][3] , multi[3][3];
   cout<<"enter the elements to the arr1 > \n";
  for(int i =0 ; i<3 ; i++){
    for(int j =0 ; j<3 ; j++){
      cin>>arr1[i][j];
    }
  }
    cout<<"enter the elements to the arr2 > \n";
  for(int i =0 ; i<3 ; i++){
    for(int j =0 ; j<3 ; j++){
      cin>>arr2[i][j];
    }
  }
  for(int i =0 ; i<3 ; i++){
    for(int j =0 ; j<3 ; j++){
      sum[i][j] = arr1[i][j] + arr2[i][j];
    }
  }
  for(int i =0 ; i<3 ; i++){
    for(int j =0 ; j<3 ; j++){
      minus[i][j] = arr1[i][j] - arr2[i][j];
    }
  }
  for(int i =0 ; i<3 ; i++){
    for(int j =0 ; j<3 ; j++){
      multi[i][j] = arr1[i][j] * arr2[i][j];
    }
  }
  cout<<"the values of addition > \n";
  for(int i =0 ; i<3 ; i++){
    for(int j =0 ; j<3 ; j++){
    cout<<sum[i][j]<<" ";
    }
   cout<<endl;
  }
  cout<<"the values of subtractions > \n";
  for(int i =0 ; i<3 ; i++){
    for(int j =0 ; j<3 ; j++){
    cout<<minus[i][j]<<" ";
    }
   cout<<endl;
  }
  cout<<"the values of multiplication > \n";
  for(int i =0 ; i<3 ; i++){
    for(int j =0 ; j<3 ; j++){
    cout<<multi[i][j]<<" ";
    }
   cout<<endl;
  }
 return 0;
}
```
### 22. Write a program in C to find transpose of a given matrix.*/
```
#include <iostream>
using namespace std;

int main(){
  int r, c;
  cout << "Enter the number of rows: ";
    cin >> r;
  cout << "Enter the number of columns: ";
    cin >> c;
  int arr[r][c];
  int tranpose[c][r];
   cout<<"enter the arrays elements > \n";
   for(int i = 0 ;i<r ;i++){
    for(int j = 0 ; j < c ;j++){
      cin>>arr[i][j];
    }
   }
   cout<<"the orignal matrix \n";
   for(int i =0 ; i < r ; i++){
    for(int j =0 ; j < c ; j++){
      cout<<arr[i][j]<<" ";
    }
    cout<<endl;
   }
   for(int i=0; i<r ; i++ ){
    for(int j =0 ; j<c;j++){
      tranpose[j][i] = arr[i][j];
    }
   }
     cout<<"the tranpose of the matrix is > \n";
   for(int i =0 ; i < r ; i++){
    for(int j = 0;j< c ;j++){
      cout<<tranpose[j][i]<<" ";    
    }
     cout << endl;
   }   
 return 0;
}
```
### 24. Write a program in C to find the sum of left diagonals of a matrix*/
```
#include <iostream>
using namespace std;

int main(){
  int n;
  cout << "enter the size of the square matrix (n x n) >>  ";
    cin >> n;
  int arr[n][n]; 
  cout << "enter the elements of the matrix:\n";
  for (int i = 0; i < n; i++){
    for (int j = 0; j < n; j++){
        cin >> arr[i][j];
    }
  }
  int sum = 0;
    for (int i = 0; i < n; i++){
      sum += arr[i][i]; 
    }
  cout << "left diagonal elements are >\n";
    for (int i = 0; i < n; i++){
      cout << arr[i][i] << " "; 
    }
  cout << endl;

  cout << "sum of left diagonal elements > " << sum << endl;

  return 0;
}
```
### 25. Write a program in C to find sum of rows an columns of a Matrix*/
```
#include <iostream>
using namespace std;

int main(){
  int r , c;
  int SumRows[r] , SumCol[c];
  cout<<"enter the amont of rows > ";
  cin>>r; 
  cout<<"enter the amount of col > ";
  cin>>c;
  int arr[r][c];
  for(int i = 0 ; i<r ; i++){
    for(int j = 0 ; j<c ; j++){
      cin>>arr[i][j];
    }
  }
  for(int i = 0 ; i < r ; i++){
    SumRows[i] = 0;
  } 
  for(int j =0 ; j<c;j++){
    SumCol[j] = 0;
  }
  for(int i =0 ; i<r;i++){
    for(int j = 0 ; j<c;j++){
      SumRows[i] += arr[i][j];
      SumCol[j] += arr[i][j];
    }
  }
  cout<<"the matrix is > \n";
  for(int i = 0 ; i<r ; i++){
    for(int j =0 ; j<c;j++){
      cout << arr[i][j]<<" ";
    }
  cout<<endl;
  }
  for(int i =0 ; i <r ; i++){
    cout<<"Sum of Rows > "<<i<<" : "<<SumRows<< endl;
  }
  for(int j =0 ; j <c ; j++){
    cout<<"Sum of col > "<<j<<" : "<<SumCol<< endl;
  }
 return 0;
}
```
### 26. Write a program in C to print or display the lower triangular of a given matrix.
### 27. Write a program in C to print or display upper triangular matrix*/
```
#include <iostream>
using namespace std;

int main(){
int n;
cout << "enter the size of the square matrix (n x n) > ";
cin >> n;
  int matrix[n][n];
  cout << "enter the elements of the matrix >\n";
  for (int i = 0; i < n; i++){
    for (int j = 0; j < n; j++){
    cin >> matrix[i][j];
    }
  }
  cout << "\nlower triangular matrix > \n";
  for (int i = 0; i < n; i++){
    for (int j = 0; j < n; j++){
      if (j <= i){
       cout << matrix[i][j] << " ";
      } else {
          cout << "0 ";
        }
    }
  cout << endl;
  }

  return 0;
}
```
### // upper triangular matrix
```
#include <iostream>
using namespace std;

int main(){
int n;
cout << "enter the size of the square matrix (n x n) > ";
cin >> n;
 int matrix[n][n];
 cout << "enter the elements of the matrix >\n";
  for (int i = 0; i < n; i++){
    for (int j = 0; j < n; j++){
    cin >> matrix[i][j];
    }
  }                                                                                   
  cout << "\nupper triangular matrix > \n";
  for (int i = 0; i < n; i++){
    for (int j = 0; j < n; j++){
      if (j >= i){
       cout << matrix[i][j] << " ";
      } else{
          cout << "0 ";
        }
    }
  cout << endl;
  }

  return 0;
}
```
### 28. Write a program in C to calculate determinant of a 3 x 3 matrix.*/
```
#include <iostream>
using namespace std;

int main() {
int matrix[3][3];

cout << "enter the elements of the 3x3 matrix >\n";
 for (int i = 0; i < 3; i++){
    for (int j = 0; j < 3; j++){
      cin >> matrix[i][j];
    }
}
int determinant = matrix[0][0] * (matrix[1][1] * matrix[2][2] - matrix[1][2] * matrix[2][1]) -matrix[0][1] * (matrix[1][0] * matrix[2][2] - matrix[1][2] * matrix[2][0]) +matrix[0][2] * (matrix[1][0] * matrix[2][1] - matrix[1][1] * matrix[2][0]);
 cout << "he determinant of the matrix is: " << determinant << endl;
return 0;
}

```
### 29. Write a program in C to accept two matrices and check whether they are equal.*/
```
#include <iostream>
using namespace std;

int main(){
int r , c;
 cout<<"enter the rows > ";
  cin>>r;
 cout<<"enter the colume > ";
  cin>>c;
int arr1[r][c];
int arr2[r][c];
cout<<"enter the elements for arr1> \n";
 for(int i = 0; i<r;i++){
   for(int j = 0 ; j<c;j++){
    cin>>arr1[i][j];
    }
  }
cout<<"enter the elements for arr2> \n";
 for(int i = 0; i<r;i++){
   for(int j = 0 ; j<c;j++){
    cin>>arr2[i][j];
    }
  }
bool areEqual = true;
  for (int i = 0; i < r; i++){
    for (int j = 0; j < c; j++){
      if (arr1[i][j] != arr2[i][j]){
        areEqual = false; 
      break; 
    }
  }
  if (!areEqual){ 
    break;
    }
  }
  if (areEqual){
  cout << "The matrices are equal.\n";
  } 
  else{
  cout << "The matrices are not equal.\n";
  }
return 0;
}
```
```
