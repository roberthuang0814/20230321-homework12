#include <stdlib.h>  
#include <stdio.h>  
int f(int);  
  
int main(){  
    int n; //定義變數n 
    scanf("%d",&n); //讀取一個整數，將其存在n中 
    printf("%d\n",f(n)); //輸出函數f(n) 
}   
  
int f(int n){  //定義f遞迴函數
    if(n==1 || n==0){ //當n的值為0或1時，函數返回n+1的值，否則，函數返回(f(n-1)+f(n/2))的值 
        return n+1;  
    }  
    else{  
        return (f(n-1)+f(n/2));  
    }  
}  
