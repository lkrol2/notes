1. html
<!DOCTYPE html>
<html>
<head>
<meta charset=utf-8 />
<title>JS Bin</title>
</head>
<body>
  <p> Ala ma kota.</p>
  <p class="warning"> Ola też ma kota</p>
  <h3 class="warning">Ala też</h3>
</body>
</html>




2. Css

body {background: yellow;
padding: 38px;
}

html { background: red;
margin: 0;
padding: 0;
}

p {
  background: blue;
  padding: 24px;
  margin: 24px;
}
h3.warning { background: white;
  padding: 24px;
  margin: 24px;
}   

p.warning: hover { background: green; }

### Wyklady Niedziela 24-03-2013.


Możemy sami definiować zmienne

Wszyskie obliczenia sa prowadzone w podwójnej precyzji tybu double.

Program rozróżnia male i Wielkie litery.

## Wyklady po przerwie.

Liczby zapisywane sa w systemie dwójkowym.

znak__mantys_wykladnik

Matysa - skończona liczba liczb

Aby zmienić dokladnosc wyswietlania liczb w MatLab.
File->Preferences->Window Command-> (**short** zminiamy na ***long***)

W Matlabie można przeciazac oberatory.

iloczyn skalarny - x1y1+x2y2+x3y3

W MATLABie nie piszemy programów tylko ***skrypt***.
Matlab jest interpreterem polecen nie potrzebuje kompilatora
Skrypty mozna uruchmiać wpisujac ich nazwe w *Window Command*

Aby zlokalizować pierwistek potrzeba kilka kroków:

f(a)f(b)<0

1. Lokalizacja

2. metoda numeryczna

a) bisekcja

    x1=(b-a)/2 /|f(x)|<E
  
    f(a)f(xi)>0
    
    f(xi)f(b)<0
    
    a=x2
    
b) metoda iteracji prostej
  
    f(x)=0
    
    x=g(x)
    
    xn+1=y(xn)
    
    x2=xp
    
c) regula falsi 
  
    patrzymy w kórym przedziale jest pierwiastek i puszczam sieczna
    
d) Metoda sieczna
  
e) Metoda Newtona-Raphsona - styczna
  
    f(x+h)=f(x)+1/1!hf'(x)+1/2!hf''(x)...
    
    f(x+x1-x)=f(x)+hf'(x)=0
    
    0=f(x+x1-x)=f(x)+hf'(x) --> x2=x-(f(x)/f'(x))
    
    
  
## Petla w Matlab'ie
  
  Petla FOR: 
  
    for s=0.0:0.01:1.0
        disp(s)
    end

  Warunek IF:
  
    r=5
    c=5
    
    if r == c
      disp('sylwek');
      else
         disp('zonk');
      end
