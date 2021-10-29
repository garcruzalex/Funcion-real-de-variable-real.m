%Octave Script
%Title            :Función 3 
%Description      :Script para recordar la resolucion de funcion real de variable real y su representación gráfica  
%Autor            :Garcia Cruz Alejandro
%Version          :1
%Date             :28/10/2021
%Notes            :http://octaveintro.readthedocs.io/en/latest/index.html

clear 

%Iniciar paquete symbolic
pkg load symbolic 
syms t

%dominio de la función
x=1:1:5

%función a plotear 
ht= (t)/(2-t)
ezplot(ht)
ylabel('y')
xlabel('x')
title('dominio (-oo,2)U(2,oo) rango [-oo,-1)U(-1,oo)') 
 20  funciontrozos1.m 
@@ -0,0 +1,20 @@
%Octave Script
%Title            :Funcion a trozos 1
%Description      :Script para recordar la resolucion de funciones a trozos 
%Autor            :Garcia Cruz Alejandro
%Version          :1
%Date             :28/10/21
%Notes            :http://octaveintro.readthedocs.io/en/latest/index.html

clear

%La función f, con dominio en todo R 
%Calcula f(-1),f(5) y f(6)
f=@(x) (-x+2).*(x<-1)+(x).*(-1<=x).*(x<=2)+(2).*(x>2);
f(-1)
f(5)
f(6)
%Estudia la continuidad de f
f(3)
f(5)
fplot(@(x)(-x+2).*(x<-1)+(x).*(-1<=x).*(x<=2)+(2).*(x>2),[-5,5])
 20  funciontrozos2.m 
@@ -0,0 +1,20 @@
%Octave Script
%Title            :Funcion a trozos 2
%Description      :Script para recordar la resolución de funciones a trozos 
%Autor            :Garcia Cruz Alejandro
%Version          :1
%Date             :28/10/21
%Notes            :http://octaveintro.readthedocs.io/en/latest/index.html

clear

%funcion trozos
%si f:D?I | f(x)=(sqrt=0 si 0<=x<=1)(2-x si 1<x<=2)
f=@(x) (x).*(0<=x).*(x<=1)+(2-x).*(1<x).*(x<=2);
f(-1)
f(5)
f(6)
%estudia la continuidad de f
f(3)
f(5)
fplot(@(x)(x).*(0<=x).*(x<=1)+(2-x).*(1<x).*(x<=2),[0,2]) 
 21  graf1.m 
@@ -0,0 +1,21 @@
%Octave Script
%Title            :Función 1
%Description      :Script para recordar la resolución de función real de variable real y su representación gráfica 
%Autor            :Garcia Cruz Alejandro
%Version          :1
%Date             :28/10/21
%Notes            :http://octaveintro.readthedocs.io/en/latest/index.html

%Función 1
%f(x)=1+? x-4
clear

pkg load symbolic
syms x
x=[4:1:15]
y= 1+(sqrt(x-4));
plot(x,y)
hold on
ylabel('y')
xlabel('x')
title('dominio [4,oo), rango [1,+oo), minimo (4,1)')
 25  graf2.m 
@@ -0,0 +1,25 @@
%Octave Script
%Title            :Función 2
%Description      :Script para recordar la resolucion de función real de variable real y su representación gráfica   
%Autor            :Garcia Cruz Alejandro
%Version          :1
%Date             :28/10/21
%Notes            :http://octaveintro.readthedocs.io/en/latest/index.html


%Regla de correspondencia(función)
%fx= (1+x.^2)

clear

pkg load symbolic
syms x
%dominio de la función
x=[-5:1:5]
%función a plotear
y=1+x.^2
plot(x,y)
grid on
ylabel('y')
xlabel('x')
title('dominio (-oo,oo), rango [1,+oo), vertice(0,1)') 
 19  graf4.m 
@@ -0,0 +1,19 @@
%Octave Script
%Title            :Grafica 4
%Description      :Script para recoradar la resolucion de funcion real de variable real  
%Autor            :Garcia Cruz Alejandro
%Version          :1
%Usage
%Notes 

clear

%dominio de la función
x=-5:1:-1;

%Regla de correspondencia(función)
fx= (x.^2)+(6*x)

%plotear función
plot(x, fx)

 27  graf5.m 
@@ -0,0 +1,27 @@
%Octave Script
%Title            :Función 5
%Description      :Script para recordar la resolucion de funcion real de variable real y su representación gráfica   
%Autor            :Garcia Cruz Alejandro
%Version          :1
%Date             :28/10/21
%Notes            :http://octaveintro.readthedocs.io/en/latest/index.html


%Función de valor absoluto
%g(z)=|z^3|

clear

%Cargar paquete symbolic
pkg load symbolic
syms z

%dominio de la función
z=[-20:1:20];
%Función a plotear 
y=abs(z.^3);
plot(y)
grid on
ylabel('y')
xlabel('x')
title('raiz(0,0), dominio zE R, rango [0,oo)') 
 23  graf6.m 
@@ -0,0 +1,23 @@
%Octave Script
%Title            :Función 6
%Description      :Script para recordar la resolucion de función real de variable real y su representación gráfica  
%Autor            :Garcia Cruz Alejandro
%Version          :1
%Date             :28/10/21
%Notes            :http://octaveintro.readthedocs.io/en/latest/index.html

clear 

%Iniciar paquete symbolic
pkg load symbolic 
syms t

%dominio de la función
x=1:1:5

%función a plotear 
ht= (t-1)/(t-2)
ezplot(ht)
ylabel('y')
xlabel('x')
title(' dominio (-oo,o2)U(2,oo), rango [-oo,1)U(1,oo)') 
 24  graf7.m 
@@ -0,0 +1,24 @@
%Octave Script
%Title            :Grafica 7
%Description      :Script para recordar la resolucion de funcion real de variable real y su representación gráfica  
%Autor            :Garcia Cruz Alejandro
%Version          :1
%Date             :28/10/21
%Notes            :http://octaveintro.readthedocs.io/en/latest/index.html

clear 

%Iniciar paquete symbolic
pkg load symbolic 
syms x

%dominio de la función
r=[-5:1:5];
%Función a plotear
f=(2*x.^2+3*x)/(x.^2+4*x+5);
ezplot(f)
ylabel('y')
xlabel('x')



 24  graf8.m 
@@ -0,0 +1,24 @@
%Octave Script
%Title            :Función de cuarto grado
%Description      :Script para recordar la resolución de función real de variable real y su representación gráfica   
%Autor            :Garcia Cruz Alejandr
%Version          :1
%Date             :28/10/21
%Notes            :http://octaveintro.readthedocs.io/en/latest/index.html

%Función de cuarto grado
%f(x)x^4+6x^3+9x^2-1

clear
%iniciar paquete symbolic
pkg load symbolic
syms x
x= linspace(-50,50);
disp ('valor de la funcion');
disp('((2*x.^2+3*x)./(x.^2+4*x+5)');
fx=((x.^4)+(6*x.^3)+((9*x.^2)-1));
semilogy (x,fx);
grid on;
ylabel('y')
xlabel('x')
title('dominio xE R, rango [-1,+oo), minimos(-3,-1)(0,-1), maximo(-3/2,65/16)') 
