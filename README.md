# program-to-find-the-maximum-and-minimum-element-of-an-array

#include<iostream>
  using namespace std;
    int main(){
        int n;
        cout<<"enter the size of array : "<<"\n";
        cin>>n;
        
        int arr[n];
        for(int i=0; i<n;i++){
            cout<<"enter the elements of array  "<<i+1<<"\n";
            cin>>arr[i];
        }
        
        
        cout<<"elements are : "<<"\n";
         for(int i=0;i<n;i++){
             cout<<arr[i]<<" ";
         }
         
         int max=arr[0];
         int min=arr[0];
         
         for(int i=0;i<n;i++){
             if(max<arr[i]){
                 max=arr[i];
             }
              if(min>arr[i]){
                 min=arr[i];
             }
             

         }
             cout<<"maximum element is : "<<max<<"\n";
             cout<<"minimum element is : "<<min<<"\n";
        return 0;
    }
