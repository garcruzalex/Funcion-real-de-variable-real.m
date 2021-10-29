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

