#include<stdio.h><br/>
int main(){<br/>
    int arr[6][6];<br/>
    for(int i=0;i<6;i++){<br/>
        for(int j=0;j<6;j++){<br/>
            scanf("%d",&arr[i][j]);<br/>
        }<br/>
    }<br/>
    int arr2[4][4];<br/>
for(int i=0;i<4;i++){<br/>
    int sum = 0;<br/>
    for(int j=0;j<4;j++){<br/>
        sum = arr[i][j]+arr[i][j+1]+arr[i][j+2]<br/>
                +arr[i+1][j+1]<br/>
                +arr[i+2][j]+arr[i+2][j+1]+arr[i+2][j+2];<br/>
                arr2[i][j] = sum;<br/>
    }<br/>
}<br/>
 signed int great = arr2[0][0];<br/>
for(int i=0;i<4;i++){<br/>
    for(int j=0;j<4;j++){<br/>
        if(great<arr2[i][j]){<br/>
            great = arr2[i][j];<br/>
        }<br/>
        else{<br/>
            continue;<br/>
        }<br/>
    }<br/>
}<br/>
printf("%d",great);<br/>
    return 0;<br/>
}<br/>
