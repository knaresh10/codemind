 [Sort an array of 0s and 1s](https://thecodemind.io/app/discription.php?pageCategory=c3pzTm1NaHFsYWVCeFpGMVpkTDloZz09&Tid=eDdqYzJidml5cGFLMEhQNThJMHowdz09&Pid=Wm5jT3h4b1Z3bVh4YVg2bU5xN2M1UT09&Course=bCt3WlAvSHJ0UFZNQ1lYanRHWm5lQT09&Technology=VytvRXpaWXBDM1pCeDVxWTd6QkQzZz09&Topic=SXVxYURxU2Y1N2VDd2E3d1hpVExMZz09)
 
 ```c
 #include<stdio.h>
int main() {
    int n;
    scanf("%d",&n);
    int zerocnt = 0, onecnt = 0;
    for(int i = 0; i < n; i++) {
        int tmp; 
        scanf("%d",&tmp);
        if(tmp == 0) zerocnt++;
        else onecnt++;
    }
    while(zerocnt--) printf("%d ",0);
    while(onecnt--) printf("%d ", 1);
    return 0;
}
```
