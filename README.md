#include<stdio.h>
int main(){
    int arr[6][6];
    for(int i=0;i<6;i++){
        for(int j=0;j<6;j++){
            scanf("%d",&arr[i][j]);
        }
    }
    int arr2[4][4];
for(int i=0;i<4;i++){
    int sum = 0;
    for(int j=0;j<4;j++){
        sum = arr[i][j]+arr[i][j+1]+arr[i][j+2]
                +arr[i+1][j+1]
                +arr[i+2][j]+arr[i+2][j+1]+arr[i+2][j+2];
                arr2[i][j] = sum;
    }
}
 signed int great = arr2[0][0];
for(int i=0;i<4;i++){
    for(int j=0;j<4;j++){
        if(great<arr2[i][j]){
            great = arr2[i][j];
        }
        else{
            continue;
        }
    }
}
printf("%d",great);
    return 0;
}
