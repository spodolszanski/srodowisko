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
zadanie 15. Wczytuje liczbe calkowita n>=0 a nastepnie n liczb rzeczywistych (double %lf) i drukuje te 
liczby w trzech kolumnach w taki sposob, zeby zachowac krycie (tzn. kropka dziesietna zawsze byla w tych 
samych kolumnach) np gdy uzytkownik:
poda 7 0.12 -31,5 2,5 -59,01 26,4 -12,0 8,3 
kol1   0,12  -59,01   8,3
kol2  -31,50  26,40
kol3   2,50   -12,00

Mozna zakładac ze liczby naleza do przedzialu (-100,100). Zeby wydrukowal l. rzeczywista na o dl. 6 znakow 
z 2 cyframi po kropce nalezy w komendzie "printf" uzyc formatu "%6.2 lf" ./zad < plik_z_danymi --> przekierowuje 
nas do pliku z danymi np. "n"

```c
main () {
  int n,i;
  printf("Podaj n\n");
  scanf("%i", &n);
  /*deklaracja tablicy*/
  double tab[n];
     /*petla wczytujaca dane z tablicy*/
    for (i=0; i<n; i++)
      scanf("%lf\n", &tab[i]);
  /*petla wpyisujaca dane z tablicy*/
    for (i=0; i<n; i++) {
    printf("%2.3lf\n", tab[i]);
    if (i%3==2)
      printf ("\n");
    }
}

```

zadanie 16.  Napisz program ktory wczyta od uzytkownia dane do piecioelementowej tablicy liczb calkowitych, 
a nastepnie wypisze na ekran sume jej elementow.

```c
main () {
  int i,j,suma;
  //nadawanie poczatkowej wartosci zmiennej suma
  suma=0;
  //wczytywanie ilosci liczb
  printf("Podaj liczbe\n");
  scanf("%i", &j);
  //deklaracja tablicy
  int tab[j];
  //wczytywanie liczb do tablicy
  for (i=0 ; i<j ; i++)
    scanf("%i", &tab[i]);
  //wyliczanie wartosci sumy
  for (i=0; i<j; i++){
    /* printf("%i\n", tab[i]);*/
  suma=suma+tab[i];
  }
  //wyswietlanie wyniku
  printf("Wynik to %i \n ", suma);
}
```

zadanie 17. Napisz program ktory wczyta od uzytkownika dane do piecioelementowej tablicy liczb calkowitych, 
a nastepnie przestawu jej pierwszy element z ostatnim i wypisze cala tablice na ekran.

```c
main () {
  int i, j, tmp;
  //wczytywanie liczby elementow tablicy
  printf("Podaj liczbe calkowita: \n");
  scanf("%i", &j);
  //deklaracja tablicy
  int tab[j];
  //wczytywanie danych do tablicy
  for(i=0; i<j; i++)
    scanf("%i", &tab[i]);
  //zamiana pierwszego i piatego elementu tablicy
  tmp=tab[0];
  tab[0]=tab[4];
  tab[4]=tmp;
  //drukowanie elementow tablicy
  for(i=0; i<j; i++)
    printf("%i \n", tab[i]);

}
```

zadanie 18. Zadeklaruje dwie piecioelementowe tablice liczb calkowitych, wczyta dane do pierwszej tabel, 
a nastepnie przekopijuje dane do drugiej i wypisze na ekran zawartosc drugiej tabeli.

```c
main () {
  int i, j, tmp;
    printf("Podaj liczbe \n");
  scanf("%i", &j);
  //deklaracja tablicy
  int tablica[j];
    //deklaracja 2 tablicy
  int tab[j];
  //petla wczytujaca dane do tablicy 1
  for (i=0; i<j; i++)
    scanf("%i", &tab[i]);
  //petla kopiujaca dane z tab do tablicy
  for (i=0; i<j; i++) 
 tablica[i]=tab[i];
  //petla wypisujaca dane z tablicy
  for(i=0; i<j; i++)
    {
      printf("tablica[%i]=%i \n",i, tablica[i]);

    }
} 
```
zadanie 19. Napisz program wczytujacy dwie tablice liczb rzeczywistych (double) tej samej dlugosci 
i drukujacy ich iloczyn skalarny.

```c
main (){
  int i,b,d,k;
printf("Podaj długość  tabilcy\n");
scanf("%i", &d);
 
//deklarowanie tablicy
double tab[d];
 double tablica[d];
//petla wczytujaca tablicę
 for (i=0; i<d; i++)
  scanf("%lf", &tab[i]);
 printf("podaj dane do drugiej tablicy \n");
 for (i=0; i<d; i++)
   scanf("%lf", &tablica[i]);
 // petla wypisujaca tablice
 printf("dane z pierwszej tablicy \n");
 for (i=0; i<d; i++)
   printf("%lf\n", tab[i]);
 printf("dane z drugiej tablicy \n");
 for (i=0; i<d; i++)
 printf("%2.2lf\n", tablica[i]);  
 for (i=0; i<d; i++)
   k=k+tab[i]*tablica[i];
 printf("Wynik iloczynu skalarnego %i\n", k);
 }
```

zadanie 20. analiza programu

```c
/* kopiowanie zawartości pliku */

int main (int argc, char *argv[]) {
  FILE *fin;   /* uchwyt do pliku wejściowego */
  FILE *fout;  /* uchwyt do pliku wyjściowego */
  int c;
  //podanie dokładnie 3 argumentow!!!
  if (argc != 3) {
    printf("Użycie: %s SOURCE DEST\n", argv[0]);
    return 3;
  }
  //otwarcie pliku i co chcemy z nim zrobic (zalezy od litery np "r") tutaaj tylk czytac
  if ((fin = fopen(argv[1], "r")) == NULL) {
    printf("Nie mogę otworzyć pliku do czytania '%s'\n", argv[1]);
    return 1;
  }
  //otwarcie pliku do zapisu
  if ((fout = fopen(argv[2], "w")) == NULL) {
    printf("Nie mogę otworzyć pliku do zapisu '%s'\n", argv[2]);
    return 2;
  }
  // skad dokoad sie skopiowalo
  printf("Kopiowanie pliku: %s -> %s\n", argv[1], argv[2]);
  
// c -znaki ktore sa zawarte w pliku
  while ((c = fgetc(fin)) != EOF) {
    fputc(c, fout);
  }
  // konieczne zamkniecie obu plikow, jezli na mam zamkniecia dane z pliku sie nie zapisuja
  fclose(fin);
  fclose(fout);

  return 0;
}

```

