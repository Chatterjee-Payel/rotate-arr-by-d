# rotate-arr-by-d
class Solution{
    public:
    //Function to rotate an array by d elements in counter-clockwise direction. 
    void rotateArr(int arr[], int d, int n){
        // code here
    int arr1[n],arr2[n],m=0,f=0,w=0;
     while(d>n)
     {
         d=d-n;
     }
     int a[d];
     for(int i=0;i<d;i++){
         arr1[f++]=arr[i];
     }
     for(int i=d;i<n;i++){
         arr2[m++]=arr[i];
     }
     for(int i=0;i<m;i++){
         arr[w++]=arr2[i];
     }
     for(int i=0;i<f;i++){
         arr[w++]=arr1[i];
     }
    }
};
