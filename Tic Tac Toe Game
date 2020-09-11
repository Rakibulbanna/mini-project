#include <bits/stdc++.h>
#include <iostream>
#include <windows.h>
#include <algorithm>
#include <vector>
#include <string>
using namespace std;

/*
Created by
Rakib ul banna
SWE
*/


int display(char a1[4][4]){

   system("cls");
    printf ("\n\n");

    cout << setfill(' ') << setw(10) <<"\t      Welcome to my Tic Tac Toe Game\n";
    cout << setfill(' ') << setw(10) <<"\t   ------------------------------------\n\n";

 for (int i=0;i<3;i++){
        for (int j=0;j<3;j++){
            cout << setfill(' ') << setw(10) <<a1[i][j]<<' ';
            if (j!=2) {cout <<"\t|";}
        }
        if (i!=2){cout <<"\n\t-------------------------------------\n";}
    }

    return 0;

}
int display2(char a1[4][4]){

  // system("cls");
    printf ("\n\n\n");

    cout << setfill(' ') << setw(10) <<"\t             FINAL RESULT\n";
    cout << setfill(' ') << setw(10) <<"\t   ------------------------------------\n\n";

 for (int i=0;i<3;i++){
        for (int j=0;j<3;j++){
            (a1[i][j]=='X' || a1[i][j]=='O')? cout << setfill(' ') << setw(10) <<a1[i][j]<<' ':cout << setfill(' ') << setw(10) <<' ';
            if (j!=2) {cout <<"\t|";}
        }
        if (i!=2){cout <<"\n\t-------------------------------------\n";}
    }

    return 0;

}

int win(char a[4][4]){
bool flag=false;

int i;
for (i=0;i<3;i++){
 if (a[i][0]==a[i][1] && a[i][2]==a[i][1]){
        flag=true;
        break;
 }
}

if (flag){return a[i][0];}
else {
    bool f=false;
    int j;
    for ( j=0;j<3;j++){
        if (a[0][j]==a[1][j] && a[1][j]==a[2][j]){
            f=true;
            break;
        }
    }
if (f){return a[0][j];}
else {
    if (a[0][0]==a[1][1] && a[1][1]==a[2][2]){return a[0][0];}
    else if (a[0][2]==a[1][1] && a[1][1]==a[2][0]){return a[1][1];}
    else {
        return 0;
    }
}

}


}

int main () {
    bool r=true;
    while (r){
    set<int>v;


    int i,j,c=1;

   char a[4][4]={"123","456","789"};

    int k=9;
    int m;
    char g='X';



    for(m=0;m<9;m++) {
            if (m%2==0){g='O';}
            else {g='X';}

     system("cls");

        display(a);

        char d = win(a);
        //cout <<'\n'<<d<<endl;
        if (d == 'X'){display2(a); cout<<"\n\n\n\t\t    congratulations!!\n\t\t\t"<<"X"<<' '<<"Win\n\n"<<endl;break;}
        else if (d == 'O'){display2(a);cout<<"\n\n\n\t\t    congratulations!!\n\t\t\t"<<"O"<<' '<<"Win\n\n"<<endl;break;}
        else {

        int s;
        
     cout<<"\n\n\n\nPlease Input the turn of  -->  ";
     (m%2==0)? cout<<"O":cout<<"X";
     cout<<"  : ";


        bool x=true;

        while (x){
        cin>>s;


        if (v.find(s)!=v.end()){
                printf("\nThese Number are taken ");
               for (auto u : v){cout<<u<<' ';}

        printf("\nplease try again : ");

        }
        else { v.insert(s);x=false;}
        }


         printf("\n");

         if (s>0 && s<4){
               if (s==1){a[0][0]=g;}
               else if (s==2){a[0][1]=g;}
               else if (s==3){a[0][2]=g;}
        }
        else if (s>3 && s<7) {
                if (s==4){a[1][0]=g;}
               else if (s==5){a[1][1]=g;}
               else if (s==6){a[1][2]=g;}

        }
        else if (s>6 && s<10){
               if (s==7){a[2][0]=g;}
               else if (s==8){a[2][1]=g;}
               else if (s==9){a[2][2]=g;}
        }
        system("cls");

        display(a);


    }


}
if (m==9){
    int z=win(a);
        if (z>0){cout<<"\n\n\n\t\t    congratulations!!\n\t\t\t"<<z-1<<' '<<"Win\n\n"<<endl;}
else {printf ("\n\n\t\tGame is draw!!!!\n\n");}
}
printf("\nDo you want to play new game?\npress 1\nelse press 2\n");
int q;cin>>q;
if (q!=1){r=false;}
}
}

