# Reto_11
### Desarrolle un programa que permita realizar la suma/resta de matrices. 

```phyton
matriz_a=[[1,1,2],[3,4,2],[3,6,3],[1,2,3]]
matriz_b=[[8,6,3],[2,6,9],[2,6,7],[3,6,8]]
comparador=True
contador=len(matriz_a)
if len(matriz_a)==len(matriz_b):
    for i in range(len(matriz_a)):
        for j in range(len(matriz_a[i])):
            if comparador==False:
                break
            comparador=(len(matriz_a[i])==len(matriz_b[i]))
    if comparador==False:
        print("Matriz de diferente dimension")
    elif comparador:
        matriz_suma=[[matriz_b[i][j]+matriz_a[i][j] for j in range(0,(len(matriz_a[0])))]for i in range(0,len(matriz_a))]  
        print(matriz_suma)   
else:
    print("Matriz de diferente dimension")
```
### Desarrolle un programa que permita realizar el producto de matrices. El programa debe validar las condiciones necesarias para ejecutar la operación.

```phyton
#Desarrolle un programa que permita realizar la suma/resta de matrices. 
matriz_a=[[1,1,1],[3,4,2],[3,6,3],[1,2,3],[2,6,7]]
matriz_b=[[8,6,3,9],[2,6,9,6],[2,6,74,34]]
matriz_punto=[[0 for i in range(len(matriz_b[0]))] for i in range(len(matriz_a))]
comp_a=len(matriz_a[0])
comp_b =len(matriz_b[0])  
comparador=True
for i in range(len(matriz_a)):
        if comparador==False:
            print("Matriz Incompatible")
            break
        comparador=(comp_a==len(matriz_a[i]))
        comp_a=len(matriz_a[i])  
if comparador:
    for i in range(len(matriz_b)):
            if comparador==False:
                print("matriz incompatible")
                break
            comparador=(comp_b==len(matriz_b[i]))
            comp_b=len(matriz_b[i])  
    if len(matriz_a[0])==len(matriz_b):
        for i in range(len(matriz_a)): 
            for j  in range(len(matriz_b[0])):
                for k in range(len(matriz_a[0])):
                    matriz_punto[i][j]=matriz_a[i][k]*matriz_b[k][j]

print(matriz_punto)
```
