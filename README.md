# TemperatureConverter

#include<stdio.h>
void celsius(float cel){
 float f=(cel*9/5) + 32;
 float k=cel + 273.15;
  printf("Temperature in Fahrenheit is %.2f\n",f);
  printf("Temperature in kelvin is %.2f\n",k);
}
void fahrenheit(float feh){
  float c=(feh-32)*5/9;
  float ke=(feh - 32)*5/9 + 273.15;
  printf("Temperature in Celsius is %.2f\n",c);
  printf("Temperature in kelvin is %.2f\n",ke);
}
void kelvin(float kel){
  float c=kel - 273.15;;
  float feh=(kel - 273.15)*9/5 + 32;
  printf("Temperature in Celsius is %.2f\n",c);
  printf("Temperature in Fahrenheit is %.2f\n",feh);
}
int main(){
  int ch;
  float cel,feh,kel;
  printf("Temperature Converter:-\n");
  printf("1.Celsius to Fahrenheit and Kelvin\n");
  printf("2.Fahrenheit to Celsius and Kelvin\n");
  printf("3.Kelvin to Celsius and Fahrenheit\n");
  printf("Enter your choice(1 or 2 or 3):");
    scanf("%d",&ch);
    if(ch==1){
    printf("Enter temperature in Celsius :");
    scanf("%f",&cel);
    celsius(cel);
  }
  else if(ch==2){
     printf("Enter Temperature in Fahrenheit :");
     scanf("%f",&feh);
     fahrenheit(feh);
  }
  else if(ch==3){
      printf("Enter Temperature in kelvin :");
      scanf("%f",&kel);
      kelvin(kel);
  }
  else{
    printf("Invalid choice:");
  }
  return 0;
}
