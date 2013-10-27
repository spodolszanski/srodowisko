#rozwiazania c

zadanie 1.  Program obliczający kwadrat i sześcian podanej liczby.
```c
main(){
  int i;
  printf("Podaj liczbe");
  scanf("%i", &i);
  printf("Kwadrat to: %i \n" , i*i);
  printf("Szescian to: %i \n", i*i*i);
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

zadanie 7.  Program wyliczający.
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

zadanie 8. zamiana na system dwojkowy

```c
main(){
int liczba=8;
int i;
int wynik[20];
printf("Podaj liczbę w systemie 10: ");
scanf("%i",&liczba);
i=0;
while(liczba!=0)
{
    wynik[i]=liczba%2;
    printf(" RESZTA %i przez 2 = %i ",liczba,wynik[i]);
    liczba=liczba/2;
    printf(" PO PODZIELENIU LICZBA =  %i \n", liczba);
    i++;
}
printf("\nWYNIK:");
for(i=i-1;i>=0;i--) printf(" %i ",wynik[i]);


}
```
zadanie 9.  Napisz program, ktory wczyta liczbę całkowitą i wypisze czy jest większa od 5.

```c
main () {
  int i;
  printf("Podaj liczbe calkowita\n");
  scanf("%i", &i);
  if (i>=5)
    printf("Twoja liczba jest wieksza od 5 \n");
  else printf("Twoja liczbe jest mniejsza niz od 5 \n");

} 
```
zadanie 10. Napisz program, ktory wczyta liczbe calkowita i wypisze czy jest dodatnia, ujemna czy rowna 0.

```c
main () {
  int i;
  printf("Podaj liczbe calkowita\n");
  scanf("%i", &i);
  if (i>0)
    printf("Twoja liczba jest dodatnia\n");
  else if (i<0)
 printf("Twoja liczba jest ujemna\n");
  else 
    printf("Twoja liczba jest rowna zero\n");
  }
```
zadanie 11. Napisz program, ktory wczyta liczbe calkowita i wypisze czy jest parzysta czy nieparzysta.

```c
main () {
  int i;
  printf("Podaj liczbe calkowita:\n");
  scanf("%i", &i);
  if (i%2)
    printf("Twoja liczba jest nieparzysta\n");
  else printf("Twoja liczba jest parzysta\n");
}
```
zadanie 12. Napisz program, który wczyta dwie liczby całkowite i wypisze czy są równe.

```c
main () {
  int i,j;
  printf("Podaj pirewsza liczbe\n");
  scanf("%i", &i);
  printf("Podaj druga liczbe\n");
  scanf("%i", &j);
  if (i==j)
    printf("Twoje liczby sa rowne\n");
  else
    printf("Twoje liczby nie sa rowne\n");
}
```
zadanie 13. Napisz program, który wczyta dwie liczby całkowite i wypisze która z nich jest większa.

```c
main () {
  int i,j;
  printf("Podaj pirewsza liczbe\n");
  scanf("%i", &i);
  printf("Podaj druga liczbe\n");
  scanf("%i", &j);
  if (i>j)
    printf("Pierwsza liczba jest wiekasza od drugiej\n");
  else
    printf("Druga liczba jest wieksza od pierwszej\n");
}
```
zadanie 14. Napisz program, który poda wynik dwudziestu kwadratów.

```c
main () {
  int suma,i;
  suma=0;
  for(i=1; i<=20; i++) 
    suma=suma+i*i;
  printf("wynik sumy dwudziestu kwadratow to: %i\n", suma);
}
```

