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

<br>clc
<br>format compact
<br>format long
<br>s=0;
<br>for n=0:10
<br>    s=s+(4/(8*n+1)-2/(8*n+4)-1/(8*n+5)-1/(8*n+6))/16^n;
<br>    abs(s-pi)
<br>end


***
## My fun

<br>function f1 = myfun(x)
<br>f1 =x.^3-2*x-5;
<br>end
***
### fzero
<br>clc
<br>fzero(@sin,3);
<br>fzero(@cos,[1 2]);
<br>f=@(x)x.^3-2*x-5;
<br>fplot(f,[-2 3])
<br>fzero(f,-8)
<br>roots([1 0 -2 -5])
***
###zadanie

<br>clc
<br>format compact
<br>format long
<br>s=0;
<br>x=0:10;
<br>y=[];
<br>for n=0:10
<br>    s=s+(4/(8*n+1)-2/(8*n+4)-1/(8*n+5)-1/(8*n+6))/16^n;
<br>    ba=abs(s-pi);
<br>    y=[y,ba];
    
<br>end
<br>semilogy(x,y,'o')
<br>title('blad absolutny przyblizenia liczby \pi')
<br>xlabel('N')
<br>ylabel('\pi-S_N|')
****
### zadanie NEWTON

<br>format compact _%zwarte linie%_
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
