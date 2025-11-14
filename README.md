# EX 7 : THREE DIMENSIONAL TRANSFORMATIONS

## AIM :
 
 To implement the various transformations on three dimensional odjects using a c coding.

## EQUIPMENT REQUIRED:

●	Hardware: Personal Computer (PC)

●	Software: C Compiler

## ALGORITHM :


   Step 1 : Start.

   Step 2 : Draw an image with default parameters.

   Step 3 : Get the choice from user.

   Step 4 : Get the parameters for transformation.

   Step 5 : Perform the transformation.

   Step 6 : Display the output.

   Step 7 : Stop.

## Program :
```
#include<stdio.h> 
#include<conio.h> 
#include<graphics.h> 
#include<math.h> 
int maxx,maxy,midx,midy; 
void axis() 
{ 
getch(); 
cleardevice(); 
line(midx,0,midx,maxy); 
line(0,midy,maxx,midy); 
} 
void main() 
{ 
int gd,gm,x,y,z,o,x1,x2,y1,y2; 
detectgraph(&gd,&gm); 
initgraph(&gd, &gm,"c:\\turboc3\\bgi");

setfillstyle(0,getmaxcolor()); 
maxx=getmaxx(); 
maxy=getmaxy(); 
midx=maxx/2; 
midy=maxy/2; 
axis(); 
bar3d(midx+50,midy-100,midx+60,midy-90,5,1); 
printf("Enter Translation Factor"); 
scanf("%d%d%d",&x,&y,&z); 
axis(); 
printf("after translation"); 
bar3d(midx+(x+50),midy-(y+100),midx+x+60,midy-(y+90),5,1); 
axis(); 
bar3d(midx+50,midy+100,midx+60,midy-90,5,1); 
printf("Enter Scaling Factor"); 
scanf("%d%d%d",&x,&y,&z); 
axis(); 
printf("After Scaling"); 
bar3d(midx+(x*50),midy-(y*100),midx+(x*60),midy-(y*90),5*z,1); 
axis(); 
bar3d(midx+50,midy-100,midx+60,midy-90,5,1); 
printf("Enter Rotating Angle"); 
scanf("%d",&o); 
x1=50*cos(o*3.14/180)-100*sin(o*3.14/180); 
y1=50*cos(o*3.14/180)+100*sin(o*3.14/180); 
x2=60*sin(o*3.14/180)-90*cos(o*3.14/180); 
y2=60*sin(o*3.14/180)+90*cos(o*3.14/180); 
axis(); 
printf("After Rotation about Z Axis"); 
bar3d(midx+x1,midy-y1,midx+x2,midy-y2,5,1); 
axis(); 
printf("After Rotation about X Axis"); 
bar3d(midx+50,midy-x1,midx+60,midy-x2,5,1); 
axis(); 
printf("After Rotation about YAxis"); 
bar3d(midx+x1,midy-100,midx+x2,midy-90,5,1); 
getch(); 
closegraph(); 
}
```


## Output :

<img width="810" height="593" alt="image" src="https://github.com/user-attachments/assets/82b8cf12-69de-4a18-8133-df718bc19ce7" />

<img width="832" height="565" alt="image" src="https://github.com/user-attachments/assets/a961ecb4-ff9e-4ad1-92df-2c22df757a0a" />

<img width="801" height="575" alt="image" src="https://github.com/user-attachments/assets/8ae842fb-c295-4ae8-9573-96dbf15fa965" />

<img width="812" height="558" alt="image" src="https://github.com/user-attachments/assets/edb991e7-39e0-47df-9c5f-40d397c089e3" />

<img width="811" height="587" alt="image" src="https://github.com/user-attachments/assets/ccc2b34b-5fa1-4180-90d8-47c3690b8cc6" />

<img width="800" height="560" alt="image" src="https://github.com/user-attachments/assets/c071b833-2bb5-45f0-a481-b19b3d2bbb4c" />

<img width="811" height="590" alt="image" src="https://github.com/user-attachments/assets/ed09b6c0-8f8c-4b49-9b8f-e52ccee6562c" />

<img width="797" height="590" alt="image" src="https://github.com/user-attachments/assets/aaeb67d4-0e9e-4306-ba43-a1246c5035e6" />



## Result :
Thus the program was executed and the output was obtained successfully.

