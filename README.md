# yuyaya19.github.com
Just another
#include<stdio.h> 
#include<string.h>
#include<math.h> 
#include<stdlib.h>
#define N 10 //________________________________________________________________________________________________________________ 
void blessing1(void); 
void blessing2(void);
void blessing3(void);
void blessing4(void); 
void blessing5(void);
void blessing6(void);
void blessing7(void);
void PrintHeart(void);
float ff(float x, float y, float z);
float hh(float x, float z);
long f=0;
char randk();
char s[10]="color ";
//________________________________________________________________________________________________________________
int main()
{ int i=0;
  puts("\n\n\n\n\n\n\n\n\n\n ");
  for(i=0; i<N; i++)
  { s[6]=randk();
    s[7]=randk();
	system(s);
	printf("\r ★十九岁生日快乐!★");
	f=0;
	while(f<81474400)f=f+1; }
	puts("\n\n\n余亚飞:\n\n\n");
	s[6]='b';
	blessing1();
	blessing2();
	blessing3();
	blessing4();
	blessing5();
	blessing6();
	blessing7();
	printf("\n\t\t\t ");
	system("PAUSE");
	system("cls");
	PrintHeart();
	printf("\n\t\t\t ");
	system("PAUSE");
	system("cls");
	printf("\n\n\n\n\n\n\n");
	printf("\t\t\t\t\t 哈哈哈 Happy birthday！！\n");
	getchar();
	return 0; } 
char randk() 
{ char a=0;
    a=(char) abs( rand()%16);
	if(a >=10) 
	{ a-=10;
	  a+=97; }
    else a+=48; 
    return a; } 
float ff(float x, float y, float z)
{ float a = x * x + 9.0f / 4.0f * y * y + z * z - 1;
  return a * a * a - x * x * z * z * z - 9.0f / 80.0f * y * y * z * z * z; } 
float hh(float x, float z) 
{ for (float y = 1.0f; y >= 0.0f; y -= 0.001f)
  if (ff(x, y, z) <= 0.0f) return y; return 0.0f; } 
void PrintHeart(void) 
{ for(float z = 1.5f; z > -1.5f; z -= 0.05f) 
{ for(float x = -1.5f; x < 1.5f; x += 0.025f) 
{ float v = ff(x, 0.0f, z); 
   if (v <= 0.0f)
   { //s[7]=randk();
    //system(s); 
	float y0 = hh(x, z);
	float ny = 0.01f;
	float nx = hh(x + ny, z) - y0;
	float nz = hh(x, z + ny) - y0;
	float nd = 1.0f / sqrtf(nx * nx + ny * ny + nz * nz);
	float d = (nx + ny - nz) * nd * 0.5f + 0.5f;
	putchar(".:-=+*#%@"[(int)(d * 5.0f)]); }
	else putchar(' '); }
	putchar('\n'); } } 
void blessing1(void)
{ s[7]=randk();
  system(s);
  printf("\n");
  puts("☆ 愿你心之所向皆可成。");
  f=0;
  while(f<214748325)
  { f=f+1; f=f-1; f=f+1; } }
void blessing2(void)
{ s[7]=randk();
  system(s);
  printf("\n");
  puts("☆ 2020年3月15日离高考仅有84天！加油呀！！！");
  f=0;
  while(f<214748325)
  {f=f+1; f=f-1; f=f+1; } }
void blessing3(void)
{ s[7]=randk();
  system(s);
  printf("\n");
  puts("☆ 所有的努力都不会白费的。");
  f=0;
while(f<214748325)
{ f=f+1; f=f-1; f=f+1; } }
void blessing4(void)
{ s[7]=randk();
  system(s);
  printf("\n");
  puts("☆ 如你所愿做个温暖向上的女孩子，不忘初心，行在现在，不惧将来");
  f=0;
while(f<214748325)
{ f=f+1; f=f-1; f=f+1; } } 
void blessing5(void)
{ s[7]=randk();
  system(s);
  printf("\n");
  puts("☆ 用尽全力往前冲吧！加油，GGN的小鱼干"); 
  f=0;
while(f<214748325)
{ f=f+1; f=f-1; f=f+1; } }
void blessing6(void)
{ s[7]=randk();
  system(s);
  printf("\n");
  puts("☆ 愿你永远热爱生活，心怀热忱，忠于自己");
  f=0;
while(f<214748325)
{ f=f+1; f=f-1; f=f+1; } }
void blessing7(void)
{ s[7]=randk();
  system(s);
  printf("\n");
  puts("☆ 最后，爱你呀，我的小鱼干，平安喜乐，万事顺遂，健健康康");
  f=0; 
while(f<214748325)
{ f=f+1; f=f-1; f=f+1; } } 








