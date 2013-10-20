#rozwiazania c

zadanie 1
```c
int main() {
int i;
int tabela[]={1,2,4,6,12};
for(i=4; i>=0; i=i-1)
printf("/i", tabela[i]);
return 0;
}
```

zadanie 2.  Napisać i uruchomić program w C, który wczytuje liczbę naturalną "n" i drukuje wartości słowem kwadratów.
```c
main () {
  int n,suma,i;
  suma=0;
  printf("Podaj liczbe n:\n");
  scanf("%i", &n);
  //  printf("Podana liczba to: %i \n Kwadraty tej liczby to: %i",n, n*n);
  for (i=1 ; i<=n; i++)
    suma=suma+i*i;
  printf("Wynik sumy to: %i\n" ,suma);
} 
```

zadanie 3.  Napisać program obliczający wartość każdego z poniższych wyrażeń.
```c
main () {
  int n1,n2,n3;
  n1=5+3*8/2-3;
  printf("n1 wynosi: %i \n",n1);
  n2=2%2+2*2-2/2;
  printf("n2 wynosi: %i \n",n2);
  n3=2*4*(5+9/2);
  printf("n3 wynosi: %i \n",n3);
}
```

zadanie 4.  W miejsce kropek"..." wpisz kod tak, aby powstał działający program. Program wypisuje liczby z tablicy tabela [], w odwrotnej kolejności, takiej jak 12,6,4,2,1.

```c
int main() {
int tabela[]={1,2,4,6,12};
int a;
for(a=4 ; a>=0; a=a-1)
  printf("%i \n", tabela[a]);
return 0;
}
```

zadanie 5.  Program wypisujący kolejne potęgi 2, nie przekraczające 2010. FOR.
```c
main () {
  int a=1;
  for(a=1; a<=2010; a=a*2)
    printf ("%i \n", a);
}
```

zadanie 6.  Program wypisujący kolejne potęgi 2, nie przekraczające 2010. WHILE.
```c
main () {
  int a;
  a=1;
  while (a<=2010){
    printf("%i \n", a);
    a=a*2;}
  }
```

zadanie 7.  Program wyliczający sumę.
```c
main() {
  int n,suma;
  n=1;
  suma=0;
  for(n=1; n<31; n=n+1){
    if{ (n<16)
  printf ("Aktualna liczba to:%i \n",n);

    else{ 
 printf("Aktualna liczba to:%i \n", n*2);
    }
    }
}
}
```

