# Analys 2



##Integral verktyg

**Fem steg för att lösa $ \int \frac{a(x)}{b(x)} dx $**

1. Polynomdivition
   $$
   \int \frac{a(x)}{b(x)} dx = \int(p(x) + \frac{r(x)}{b(x)}) dx =\int p(x) dx  + \int\frac{r(x)}{b(x)} dx
   $$

2. Faktorisering av $b(x)​$ så långt som möjligt
   $$
   \int\frac{r(x)}{b(x)} dx = \int\frac{r(x)}{p_1*p_2*...*p_n} dx.
   $$

3. 

$$
\begin{alignat*}{}
&\text{Faktor} \qquad (x+a) &\text{partialbråk} \quad \frac{A}{(x+a)} \\
&\text{Faktor} \qquad (x+a)^n &\text{partialbråk} \quad \frac{A_1}{(x+a)^1} + \frac{A_2}{(x+a)^2}+...+\frac{A_n}{(x+a)^n} \\
&\text{Faktor} \quad (x^2+ax+b) &\text{partialbråk} \quad \frac{Ax+B}{(x^2+ax+b)} \\
&\text{Faktor} \quad (x^2+ax+b)^n &\text{partialbråk} \quad \frac{A_1x+B_1}{(x^2+ax+b)^1} + \frac{A_2x+B_2}{(x^2+ax+b)^2}+...+\frac{A_nx+B_n}{(x^2+ax+b)^n}
\end{alignat*}
$$

4. Bestäm konstanterna
5. Lös integralerna



**Primitiva funktioner för rotenuttryck**

! Innehåller uttrycket $\sqrt{\dotsc}$ eller trigonometriska uttryck utförs speciella variabelbyten.

* Faktor $\sqrt{x+a}​$ byts mot $t=\sqrt{x+a}​$

* Faktor $\frac{\sqrt{x+a}}{\sqrt{x+b}}​$ byts mot $t =\frac{\sqrt{x+a}}{\sqrt{x+b}}​$

* Faktor Faktor $\sqrt{x^2+a}​$ byts mot $t=\sqrt{x^2+a} + x​$

* Faktor Faktor $\sqrt{a - x^2}​$ byts mot $t=\sqrt{a}  \sin(t)​$ 

* Trigonometriska bytas mot $t=tan(\frac{x}{2}) \quad ,x=2\arctan(t) \quad ,\frac{dx}{dt}=\frac{2}{t^2+1} ​$ 
  $$
  \begin{align*}
  \sin(x) = \frac{2\tan(\frac{x}{2})}{\tan(\frac{x}{2})^2+1}=\frac{2t}{t^2+1} \qquad\qquad\qquad\qquad\qquad\qquad\qquad\qquad\qquad\qquad\qquad\qquad\qquad\qquad \\
  \cos(x) = \frac{1-\tan^2(\frac{x}{2})}{\tan^2(\frac{x}{2})+1}=\frac{1-t^2}{t^2+1} \qquad\qquad\qquad\qquad\qquad\qquad\qquad\qquad\qquad\qquad\qquad\qquad\qquad\qquad 
  \end{align*}
  $$

* $\sin^2(x)​$ eller $\cos^2(x)​$ byts mot eulers formel $\sin(x) = \frac{e^{ix} - e^{-ix}}{2i}​$ , $\cos(x) = \frac{e^{ix} - e^{-ix}}{2}​$



**Riemansumma**

Dela in intervallet $[a,b]$ i $n$ st delintervall $I_k = [x_{k-1}, x_k]$

Välj sedan för varje intervall ett $\epsilon \in I_k$

* Not Väljer man $\epsilon = x_{k-1}$ får man Undertrappa
* Not väljer man $\epsilon = x_k$ får man Övertrappa

$$
R_D =\sum_{i=1}^{n} f(\epsilon_i)*(x_i-x_{i-1}) \qquad\qquad\qquad\qquad\qquad\qquad\qquad\qquad\qquad\qquad\qquad\qquad\qquad\qquad
$$



**Analysens huvudsats**
$$
\int_{a}^{b}f(x) dx = \left[F(x)\right]_a^b =F(b) - F(a) \\
$$
Om $f(x)​$ har asymptot $\epsilon \in [a,b]​$ gäller inte analysens huvudsats för $\int_{a}^{b}f(x) dx​$ istället används:
$$
\int_{a}^{b}f(x) dx = \int_{a}^{\epsilon}f(x) dx + \int_{\epsilon}^{b}f(x) dx
$$


**Konvergent integral**

Där $A​$ är ett ändligt tal, kallas integralen förkonvergent
$$
\int_{a}^{b}f(x)dx = A
$$


**Divergent integral**
$$
\int_{a}^{b}f(x)dx = \pm \infin
$$
**Jämförelse test**

Om frågan är integralen konvergent eller divergent så kan man använda detta verktyget.
$$
\text{Om} \quad 0 \le f(x) \le g(x) \quad \text{och} \quad \int_{a}^{b} g(x)dx \quad \text{Konvergent} \implies \int_{a}^{b} f(x)dx \quad \text{Konvergent}\\
\text{Om} \quad 0 \le g(x) \le f(x)\quad \text{och} \quad \int_{a}^{b} g(x)dx \quad \text{Divergent} \implies \int_{a}^{b} f(x)dx \quad \text{Divergent}\\
$$



##Applicationer till integral

**Area**
$$
A = \int_{x_1}^{x_2} h(x) dx
$$


**Volym**
$$
V = \int_{x_1}^{x_2} A(x) dx
$$
**Massan**
$$
m = \int_{x_1}^{x_2} \rho(x)*A(x) dx
$$
**Längd av kurva**
$$
L = \int_{t_1}^{t_2}\left(\left(\frac{dx}{dt}\right)^2+\left(\frac{dx}{dt}\right)^2\right)^{1/2}dt \\
$$

$$
\text{Special} \quad y = y(x) \quad \text{välj } t=x\\

L = \int_{x_1}^{x_2} \sqrt{1+(y')^2} dx \\
$$

$$
\text{Polära kordinater} \quad x = r*cos(\theta) \quad y = r*sin(\theta)  \\

L = \int_{\theta_1}^{\theta_2} \left(\left( \frac{dr}{d\theta}\right)^2 + r^2 \right)^{1/2} d\theta
$$

**Mantelarea**
$$
A_m = 2\pi \int_{x_1}^{x_2} y* \sqrt{1+(y')^2} dx
$$
**Krökningsradie**
$$
\kappa \equiv \frac{1}{R} \qquad

R =\frac{(1+(y')^2)^{3/2}}{y''}
$$
**Masscentrum**
$$
X_{cm} = \frac{1}{m}*\int_{x_1}^{x_2} x* \rho(x)*A(x) dx
$$
**Tröghetsmoment**
$$
E=\frac{I\omega^2}{2} \qquad I = \int_{x_1}^{x_2}r^2dm
$$


##Diffar

**Första ordningens diffar**
$$
y'+g(x)y = f(x)
$$

$$
I(x)=e^{G(x)} \qquad y= \frac{\int I(x)*f(x)dx}{I(x)}
$$

**Andra ordningens linjära diffar**
$$
y''+Ay'+By = f(x) \\
\text{ }\\
K.E. \quad r^2+Ar+B=0 \\
\begin{alignat*}{}
a) \quad r_1 \neq r_2 \qquad reella \quad y_h = Ae^{r_1*x} + Be^{r_2*x} \\
b) \quad r_1 = r_2 \qquad reella \quad y_h = (Ax+B)e^{r*x} \\
c) \quad r = \alpha \pm i \beta \quad img \quad y_h= e^{\alpha*x}(Asin(\beta x) + Bcos(\beta x)) \\
\end{alignat*} \\
\text{ }\\

\text{Ansättning av } y_p \\

1) \quad y_h \neq k*f(x) \\
\begin{array}{c|c}
f(x) & y_p\\ 
\hline
\text{polynom grad } n & \text{polynom grad } n \\
Ae^{k*x} & Be^{kx} \\
Asin(kx)+Bcos(kx) & Csin(kx) + Dcos(kx)
\end{array}\\
\text{ }\\

2) \quad y_h = k*f(x) \\
\begin{array}{c|c}
f(x) & y_p\\ 
\hline
Ae^{k*x} & Bxe^{kx} \\
Axe^{k*x} & Bx^2e^{kx} \\

\end{array}\\
$$
**Separabla variabler**
$$
g(y)y' = f(x) \\
\text{ } \\
\int g(y)dy = \int f(x)dx
$$
**Bernaulis ekvation**
$$
y'+g(x)y = f(x)y^n \\
\text{ } \\
Z'+(1-n)g(x)Z = (1-n)f(x) \\
I(x)=e^{G(x)} \quad Z= \frac{\int I(x)*f(x)dx}{I(x)} \\
y=Z^{\left(\frac{1}{1-n}\right)}
$$

## Serie expansioner

**Maclaurin Serier**
$$
f(x) = \sum_{i=0}^{\infin}\frac{f^{(i)}(0)}{i!}*x^{i} \qquad\qquad\qquad\qquad\qquad\qquad\qquad\qquad\qquad\qquad\qquad\qquad\qquad\qquad\qquad
$$


**Tayler Serier**

*Not om $f(x)​$ ej har kontinueliga derivator $f^{(n)}(x)​$ eller ej är kontinuerlig funkar ej maclaurin expansion

*Egenskap Om en diskontinuelig funktion är kontinuelig och har kontinueliga derivator i intervallet $(a < x < b) = I​$  kan valfri $\epsilon \in I ​$ väljas och $f(x) = \sum_{i=0}^{\infin}\frac{f^{(i)}(\epsilon)}{i!} * (x-\epsilon)^{i}​$



* Def Taylorpolynom ordo $n$ kring $a$

  
  $$
  T_a(x) = \sum_{i=0}^{n}\frac{f^{(i)}(a)}{i!}*(x-a)^{i} \qquad\qquad\qquad\qquad\qquad\qquad\qquad\qquad\qquad\qquad\qquad\qquad\qquad\qquad\qquad
  $$
  





## Bevis

### 1 Partiell integrering

$$
D\left(F*g-\int F*g' dx\right) = F*g + F*g'-F*g' = f*g
$$



### 2. Analysens huvudsats

$$
\text{Antag att } F(x) = \int_t^x f(x) dx \\
\text{ } \\
\begin{alignat*}{}
F'(x)&= \lim_{\Delta x\to 0} \left(\frac{\int_{t}^{x+\Delta x}f(x)dx-\int_{t}^{x}f(x)dx}{\Delta x}\right) \\
&= \lim_{\Delta x\to 0} \left(\frac{\int_{t}^{x}f(x)dx+\int_{t}^{x+\Delta x}f(x)dx-\int_{t}^{x}f(x)dx}{\Delta x}\right) \\
&= \lim_{\Delta x\to 0} \frac{1}{\Delta x} \int_x^{x+\Delta x}f(x)dx \\
&= \lim_{\Delta x\to 0} \left( \frac{1}{\Delta x} * \Delta x * f(x) \right) \\
&= f(x) \\
\end{alignat*} \\
$$

$$
\implies F'(x) = f(x) \text{ Så är } F(x)\text{ primitiv till } f(x) \\
F(b)-F(a) = \int_t^bf(x)dx - \int_t^af(x)dx = \int_a^bf(x)dx
$$



### 3 Längd av Kurva

$$
dL = \sqrt{(dx)^2+(dy)^2} = \left(\left(\frac{dx}{dt}\right)^2\left(\frac{dx}{dt}\right)^2\right)^{1/2}dt \\

\implies L = \int_{t_1}^{t_2}\left(\left(\frac{dx}{dt}\right)^2\left(\frac{dx}{dt}\right)^2\right)^{1/2}dt
$$

### 4  Mantelarea

$$
dL = \sqrt{1+(y')^2} dx \\
dA_m = 2\pi*y*dL = 2\pi *y*\sqrt{1+(y')^2}dx \\ 
\implies A_m = \int_{x_1}^{x_2} 2\pi *y*\sqrt{1+(y')^2}dx = 2\pi\int_{x_1}^{x_2}y*\sqrt{1+(y')^2}dx
$$

### 5 Krökningsradie

$$
y'=tan(\theta) \implies \theta = arctan(y') \\
dL = R*d\theta \implies R = \frac{dL}{d\theta} = \frac{dL}{dx} * \frac{dx}{d\theta} = \frac{dL}{dx} * \left(\frac{d\theta}{dx}\right)^{-1} \\
 = \frac{\sqrt{1+(y')^2}dx}{dx}*\left( \frac{y''}{1+(y')^2} \right)^{-1}\\
 = \sqrt{1+(y')^2}* \frac{1+(y')^2}{y''} \\
 = \frac{(1+(y')^2)^{3/2}}{y''}
$$

### 6 Tröghetsmomentet

$$
dE = \frac{V^2}{2}dm = \frac{(\omega r)^2}{2}dm \\
E = \int_k \frac{\omega^2 r^2}{2}dm = \frac{\omega^2}{2}*\int_k r^2 dm \implies I = \int_k r^2 dm
$$

### 7 Första ordningens diff

$$
\begin{alignat*}{}
y'+g(x)y=f(x) &\implies y'e^{G(x)} + g(x)ye^{G(x)} = f(x)e^{G(x)}\\
							&\implies \frac{d}{dx}\left(y'e^{G(x)}\right) = \int f(x)e^{G(x)}dx \\
							&\implies y = \frac{\int e^{G(x)}f(x)dx}{e^{G(x)}}
\end{alignat*}
$$

###8 Andra ordningens diffar

$$
y''+Ay'+By=0 \\
\text{ } \\
\begin{alignat*}{}
\text{Antag} &y=Ze^{rx} \\
&y'=Z'e^{rx}+rZe^{rx} \\
&y''= Z''e^{rx}+2rZ'e^{rx}+r^2Ze^{rx}
\end{alignat*}\\
$$

$$
\begin{alignat*}{}
y''+Ay'+By&=e^{rx}\left(Z'' + 2rZ'+r^2Z+AZ'+ArZ+BZ\right) \\
&=e^{rx}\left(Z''+Z'(2r+A)+Z\underbrace{(r^2+ar+B)}_\text{KE}\right) = 0
\end{alignat*} \\
$$

$$
\text{Då KE har dubbelrot} \\
\begin{alignat*}{}
r=-\frac{a}{2}\pm\sqrt{0} &\implies a=-2r \\
&\implies Z'' = 0 \\
&\implies Z' = A \\
&\implies Z = Ax+B \\
&\implies y=e^{rx}(Ax+B) \\
\end{alignat*} \\
$$

$$
\text{Då KE har reella rötter} \\
\begin{alignat*}{}
a \neq-2r &\implies Z' = 0 \\
&\implies Z = A \\
&\implies y=Ae^{r_1x}+Be^{r_2x} \\
\end{alignat*} \\
$$

$$
\text{Då KE har imaginära rötter } \\
\begin{alignat*}{}
r= \alpha \pm i \beta &\implies y=Ae^{r_1x}+Be^{r_2x} \\
&\implies y= Ae^{\alpha + i \beta}+Be^{\alpha - i \beta} \\
&\implies y=e^{\alpha x}\left(Ae^{i\beta}+Be^{-i\beta}\right) \\
&\implies y=e^{\alpha x}\left( Acos(\beta x) +iAsin(\beta x) + Bcos(\beta x) - iBsin(\beta x)\right) \\
& \implies y=e^{\alpha x}\left( \underbrace{(A+B)}_\text{=D}cos(\beta x) + \underbrace{i(A+B)}_\text{=E}sin(\beta x)\right) \\
&\implies y=e^{\alpha x}\left( Dcos(\beta x) + Esin(\beta x)\right) \\
\end{alignat*} \\
$$



### 9 Bernaulis ekvation

$$
y'+g(x)y=f(x)y^n \\
y=Z^{\frac{1}{1-n}} \\
y'=\frac{1}{1-n}Z^{\frac{1}{1-n}-1}*Z' = \frac{Z^{\frac{1}{1-n}}*Z'}{1-n} \\
\text{Insättning ger} \\
\frac{Z^{\frac{1}{1-n}}*Z'}{1-n}+g(x)Z^{\frac{1}{1-n}} = f(x)Z^{\frac{n}{1-n}} \\
\frac{Z'}{1-n}+g(x)Z^{\frac{1}{1-n}-\frac{n}{1-n}} = f(x) \\
Z'+(1-n)g(x)Z=(1-n)f(x)
$$

### 10 Maclaurin utveckling

$$
\begin{alignat*}{}
f(x)&=f(0)+\int_{0}^{x}f'(x)dx \\
&=f(0)+\int_{0}^{x}\left(f'(0)+\int_{0}^{x}f''(x)dx\right) dx\\
&=f(0)+\int_{0}^{x}f'(0)dx + \int_{0}^{x}\int_{0}^{x}f''(x)dxdx\\
&=f(0)+\int_{0}^{x}f'(0)dx + \int_{0}^{x}\int_{0}^{x}\left(f''(0) +\int_{0}^{x}f^{(3)}(x)dx\right)dxdx\\
&=f(0)+\int_{0}^{x}f'(0)dx + \int_{0}^{x}\int_{0}^{x}f''(x)dxdx + \int_{0}^{x}\int_{0}^{x}\int_{0}^{x}f^{(3)}(x)dxdxdx\\
&\text{ }\text{ }\vdots \\
&=f(0)=+f'(0)x+\frac{f''(0)}{2}x^2+\frac{f^{(3)}(0)}{2*3}x^3 \ldots \\
&=\sum_{i=0}^{\inf}\frac{f^{(i)}(0)}{i!}x^i

\end{alignat*}
$$

