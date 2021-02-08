# MATLAB
MATLAB cheat sheet

## Get help
```MATLAB
help [command]
```
Relationals operators: **== , ~= , <, >, <=, >=**
Logicical operators : **&&, ||**

## Useful commands
* List all variables :
>```MATLAB
>whos
>```
* Clear all variables :
>```MATLAB
>clear
>```
* Clear terminal :
>```MATLAB
>clc
>```
* Squareroot :
>```MATLAB
>sqrt(2)
>```
* Module (complex) :
>```MATLAB
>abs(5+4i)
>```
* Number of lines and columns :
>```MATLAB
>size(matrice)
>```


## Variables :
* Matrix:
```matlab
matrice=[1, 2; 3, 4]
```
Output:
```
matrice =

     1     2
     3     4
```
* Complex number:
```matlab
z=4+5i
```
Output:
```
z =

   4.0000 + 5.0000i
```
* Range:
```matlab
4:10
```
Output:
```
ans =

     4     5     6     7     8     9    10
```
## Matrix operations :
* Access (line **i** column **j**, starts at 1):
```matlab
a(i,j)
```
* Access span:
```matlab
a(i,j:k)
a(i:j,k)
a(i:j,k:l)
a(i:j,k:end)
```
* Maximum value:
```matlab
max(a)
```
* Minimum value:
```matlab
min(a)
```
* Addition:
```matlab
a+b
```
* Sum all matrix members:
```matlab
sum(a)
```
* Soustraction:
```matlab
a-b
```
* Multiplication:
```matlab
a*b
```
* Scalar multiplication:
```matlab
a.*b
```
* Power up:
```matlab
a^2
```
* Scalar power up:
```matlab
a.^2
```
* Flip:
```matlab
a'
```
* Determiant :
```matlab
det(a)
```
* Invert:
```matlab
inv(a)
```
* Concatenate (on top):
```matlab
[a;b]
```
* Concatenate (side by side):
```matlab
[a,b]
```
* Zeros filled matrix:
```matlab
zeros(4,2)
```
* Ones filled matrix:
```matlab
ones(4,2)
```
## Loops:
* For:
```matlab
for i = valeurs
instructions
end 
```
* For:
```matlab
while condition
instructions
end
```
## Conditions:
* If/else if/else:
```matlab
if condition1
instructions
elseif condition2
instructions
else 
instructions
end 
```
* Switch:
```matlab
switch expression_du_switch
 case expression_du_case
 instructions
 case expression_du_case
 instructions
 ...
 otherwise
 instructions
end

```
## Graphs:
* New graph
```matlab
figure
```
* New line ([first point], [second point]):
```matlab
plot([1,3],[4,2]);
plot([1,3],[4,2],'k','linewidth',3);
% k = black
% mx = markers only
% rx- = markers and line
```
* Allow multiple drawings on figure:
```matlab
hold on 
```
* Decorate figure:
```matlab
grid
xlabel
ylabel
title
legend
axis % Scale
```
* Sinus wave:
```matlab
t = [0 : 0.1 : 2*pi]; % angles entre 0 et 2pi, avec un pas de 0.1
s = sin (t);
plot (t,s)
```
* Surface:
```matlab
x = [-1 : 0.1 : 1];
y = [-1 : 0.1 : 1];
[X,Y]=meshgrid(x,y);
Z=X.^2-Y.^2;
surf(X,Y,Z)
```
## Fun:
* Magic square dimmension **n**
```matlab
magic(n)
```
* Pi (3.1416)
```matlab
pi
```
## Comment
```MATLAB
% this is a comment
```
