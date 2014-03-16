##zadanie 2014-02-21 18:23 

<br>2+2
<br>8^4
<br>8+ans
<br>log4
<br>log(4
<br>log(4)
<br>plot
<br>plot(x,y)
<br>plot(log4)
<br>sin(3)
<br>sin(pi/9)
<br>2*1.73/2.72^3-17.2+14./7
<br>x=-ln2.4+sgrtsin(4) -exp(3.4)/2pi
<br>x=-ln2.4+sgrtsin(4)-exp(3.4)/2pi
<br>x=-ln2.4+sgrt sin(4)-exp(3.4)/2pi
<br>x=-ln2.4
<br>x= -ln2.4
<br>-ln2.4
<br>[-ln2.4]
<br>(-ln(2.4)+sqrt(sin(4))-4*exp(3.4))/(2*pi)
<br>(-ln(2.4)+sqrt(sin(4))-4*exp(3.4)))/(2*pi)
<br>(-log(2.4)+sqrt(sin(4))-4*exp(3.4)))/(2*pi)
<br>(-log(2.4)+sqrt(sin(4)-4*exp(3.4)))/(2*pi)
<br>(sqrt4xp(12.4))/(2tan(pi*0.47))
<br>(sqrt4xp(12.4)/(2tan(pi*0.47))
<br>(sqrt4exp(12.4)/(2tan(pi*0.47))
<br>(sqrt4exp(12.4))/(2tan(pi*0.47))
<br>(sqrt4exp(12.4))/(2tan(pi*0.47)))
<br>(sqrt4*exp(12.4))/(2tan(pi*0.47)))
<br>(sqrt4*exp(12.4)/(2tan(pi*0.47)))
<br>(sqrt*4exp(12.4)/(2tan(pi*0.47)))
<br>(sqrt4exp(12.4)/(2tan*(pi*0.47)))
<br>(sqrt4*exp(12.4)/(2tan*(pi*0.47)))
<br>sqr(4*exp(12.4)/(2tan*(pi*0.47)))
<br>sqrt(4*exp(12.4)/(2tan*(pi*0.47)))
<br>sqrt(4*exp(12.4))/(2tan*(pi*0.47)))
<br>sqrt(4*exp(12.4))/(2tan*(pi*0.47))
<br>(sqrt(4*exp(12.4))/(2tan*(pi*0.47))
<br>(sqrt(4*exp(12.4))/(2*tan*(pi*0.47))
<br>(sqrt(4*exp*(12.4))/(2*tan*(pi*0.47))
<br>(sqrt*(4*exp*(12.4))/(2*tan*(pi*0.47))
<br>(sqrt*(4*exp*(12.4)))/(2*tan*(pi*0.47))
<br>(sgrt*(4*exp*(12.4)))/(2*tan*(pi*0.47))
<br>(sqrt(4*exp*(12.4)))/(2*tan*(pi*0.47))
<br>(sqrt(4*exp(12.4)))/(2*tan*(pi*0.47))
<br>(sqrt(4*exp(12.4)))/(2*tan(pi*0.47))

***
### zadanie liczba

clc
format compact
format long
s=0;
for n=0:10
    s=s+(4/(8*n+1)-2/(8*n+4)-1/(8*n+5)-1/(8*n+6))/16^n;
    abs(s-pi)
end


***
## My fun

function f1 = myfun(x)
f1 =x.^3-2*x-5;
end
***
### fzero
clc
fzero(@sin,3);
fzero(@cos,[1 2]);
f=@(x)x.^3-2*x-5;
fplot(f,[-2 3])
fzero(f,-8)
roots([1 0 -2 -5])
***
###zadanie

clc
format compact
format long
s=0;
x=0:10;
y=[];
for n=0:10
    s=s+(4/(8*n+1)-2/(8*n+4)-1/(8*n+5)-1/(8*n+6))/16^n;
    ba=abs(s-pi);
    y=[y,ba];
    
end
semilogy(x,y,'o')
title('blad absolutny przyblizenia liczby \pi')
xlabel('N')
ylabel('\pi-S_N|')
****
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
     
<br>x0=1.5;
<br>for i=1:10
<br>    x1=x0-(cos(x0)+sin(x0))/(-sin(x0)+cos(x0));
<br>    if abs(x1-x0)<10^-3
<br>        break %robi się w instrukji warunkowej%
<br>    end
<br>    x0=x1;
<br>end
<br>i
<br>x1/pi    
