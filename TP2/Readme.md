# TP2: Interpolation Numérique
>
>
## Objectif:
> En analyse numérique, une fonction f inconnue explicitement est souvent
>
> * connue seulement en certains points x0, x1, ..., xn ;
>
> * ou évaluable uniquement au moyen de l’appel a un code couteux.
> Mais dans de nombreux cas, on a besoin d’effectuer des opérations (dérivation, intégration,...) sur la fonction f.
> 
> On cherche donc a reconstruire f par une autre fonction fr simple et facile a evaluer a partir
> des données discr etes de f. On espere que le modele f' ne sera pas trop éloigné de la fonction f aux autres points.
> 
<img src="Inter.PNG"  style="width:350px;height:300px;margin-left: auto;margin-right: auto;"/>


> **Donc on va s’intéressé dans ce TP a la reconstruction de f par des polynômes**
>
## Polynome d'interpolation de Lagrange: 
> Soient $(x_0,y_0), \ldots,(x_k,y_k),\ldots ,(x_n,k_n)$ $n+1$ points deux à deux distincts, le polynôme d'interpolation de Lagrange associés à ces points supports est défini par :
> $$P_n(x)=\sum_{k=0}^{n-1} y_kL_k(x)$$

avec $L_{0}(x)=\displaystyle\frac{(x-x_1)(x-x_2)\ldots(x-x_{n})}{(x_0-x_1)(x_0-x_2)\ldots(x_0-x_{n})}$ et $L_{k}(x)=\displaystyle\frac{(x-x_1)(x-x_2)\ldots(x-x_{k-1})(x-x_{k+1})\ldots(x_0-x_{n})}{(x_k-x_0)(x_k-x_1)\ldots(x_k-x_{k-1})(x_k-x_{k+1})\ldots(x_k-x_{n})}$ pour $k\in \{1,\ldots,n\}$
>
>
> <h3 style="color:SlateBlue;"> un inconvénient de l’interplation de Lagrange est lorsqu’on ajoute un point xN+1 aux points existants X0, 1, · ·  
>, Xn , on a recours à recalculer tous les élements Li pour chaque i = 0, · · · , N+1,c’est a dire, de répeter tout le travail et donc une perte 
>de temps</h3> 

<img src="tche.PNG"  style="width:350px;height:300px;margin-left: auto;margin-right: auto;"/>
## Phenomène de Runge:
> **Dans le domaine mathématique de l'analyse numérique, le phénomène de Runge se manifeste dans le contexte de l'interpolation polynomiale, en particulier l'interpolation de Lagrange. Avec certaines fonctions (même analytiques), l'augmentation du nombre n de points d'interpolation ne constitue pas nécessairement une bonne stratégie d'approximation.**
### Exercice 2 :

<img src="equi.PNG"  style="width:350px;height:300px;margin-left: auto;margin-right: auto;"/>
> **On a vu donc que le phénomène de Runge qui se traduit par une mauvaise interpolation,lorsque l'on augmente le degré du polynôme d'interpolation de Lagrange.**

## Formule de Newton 

> **Cette méthode ne différe de l’interpolation lagrangienne que par la maniére dont le polynôme est calculé, polynôme d’interpolation qui en résulte est le même.**

### Exercice 3 :

<img src="tche.PNG"  style="width:350px;height:300px;margin-left: auto;margin-right: auto;"/>

