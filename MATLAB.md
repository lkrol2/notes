### zadanie NEWTON

format compact _%zwarte linie%_
<br>format long _%obliczenia okazują się bardziej dokladne%_
<br>clc
<br>x=-2*pi:0.1:2*pi;

<br>y=cos(x)+sin(x)
<br>x=x/pi;
<br>y1=x*0%funkcja stała wyznaczająca linię przecinającą%
<br>plot(x,y,x,y1)
<br>xlabel('x/\pi')_%podpisze taBELE BA DOLE%_

<br>x0=1.5;
<br>for i=1:5
    <br>x1=x0-(cos(x0)+sin(x0))/(-sin(x0)+cos(x0));
    <br>x1/pi
    <br>x0=x1;
<br>end
     
     
     inna wersja
     
x0=1.5;
for i=1:10
    x1=x0-(cos(x0)+sin(x0))/(-sin(x0)+cos(x0));
    if abs(x1-x0)<10^-3
        break %robi się w instrukji warunkowej%
    end
    x0=x1;
end
i
x1/pi    
