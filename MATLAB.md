### zadanie NEWTON

format compact _%zwarte linie%_
format long _%obliczenia okazują się bardziej dokladne%_
clc
x=-2*pi:0.1:2*pi;

y=cos(x)+sin(x)
x=x/pi;
y1=x*0%funkcja stała wyznaczająca linię przecinającą%
plot(x,y,x,y1)
xlabel('x/\pi')_%podpisze taBELE BA DOLE%_

x0=1.5;
for i=1:5
    x1=x0-(cos(x0)+sin(x0))/(-sin(x0)+cos(x0));
    x1/pi
    x0=x1;
end
     
