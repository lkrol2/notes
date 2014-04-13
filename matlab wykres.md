x=0:0.2:2*pi;
plot(x,sin(x));
grid on
title('Przykład wykresu:');
xlabel('x');
ylabel('sin(x)');

%przykład%wykresu%słupkowego:
x=0:0.2:2*pi;
bar(x,sin(x));
grid on



clc
format compact
global x
x=round(rand(1,10)*100)
mean(x)
[a,b,c]=statg
min(x)
max(x)




x=0:0.2:12;
y1=Bessel(1,x);
y2=Bessel(2,x);
y3=Bessel(3,x);

figure(1)
subplot(2,2,1)

h=plot(x,y1,x,y2,x,y3);

set(h,'LineWidth',2,{'LineStyle'},{'--';':';'-.'})
set(h,{'Color'},{'r';'g';'b'})

axis([0 12-0.5 1])


x=0:0.2:12;
y1=Bessel(1,x);
y2=Bessel(2,x);
y3=Bessel(3,x);

figure(1)
subplot(2,2,1)

h=plot(x,y1,x,y2,x,y3);

set(h,'LineWidth',2,{'LineStyle'},{'--';':';'-.'})
set(h,{'Color'},{'r';'g';'b'})

axis([0 12-0.5 1])

