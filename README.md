//# Linear-Search-in-2D-Array
#include<iostream>
using namespace std;
bool findelement(int a [][4],int rowsize, int colsize, int target){
    for(int i=0;i<rowsize;i++){
        for(int j=0;j<colsize;j++){
            if(a[i][j] == target) return true;
        }
    }
    return false;
}

int main(){
    int a[3][4] = {
                    {35,22,45,54},
                    {46,87,33,88},
                    {43,21,65,76}
    };
    int rowsize = 3;
    int colsize = 4;
    int target;
    cout<<"Enter target element = "<<endl;
    cin>>target;
    bool ans = findelement(a,rowsize,colsize,target);
    if(ans) cout<<"Element Present"<<endl;
    else cout<<"Element not present"<<endl;
}
