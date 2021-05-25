# mechatronics
# newthon-raphson method
x0=input('Initial value: ');
tol=input('Error percentage: ');
f=input('Function: ');
i=1;
fx(i)=x0;
 
syms x;
f1=subs(f,x,fx(i));
z=diff(f);
d=subs(z,x,fx(i));
 
ea(1)=100;
 

end
fprintf('i     fx(i)         Error aprox (i) \n');
for j=1:i;
    fprintf('%2d \t %11.7f \t %7.3f \n',j-1,fx(j),ea(j));
end
