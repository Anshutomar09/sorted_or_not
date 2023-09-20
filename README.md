# sorted_or_not
// Online C++ compiler to run C++ program online
#include <iostream>
using namespace std;
bool recursion(int arr[], int n){
    if(n==1 ||n==0){
        return true;
    }
    if(arr[0]>arr[1]){
        return false;
    }
    else
    recursion(arr+1,n-1);
    
}
int main() {
    // Write C++ code here
    int arr[5]={2,6,4,10,6};
     if(recursion(arr, 5)){
     cout<<"ARRAY IS SORTED"<<endl;
     }
     else{
         cout<<"not sorted"<<endl;
     }
    
}
