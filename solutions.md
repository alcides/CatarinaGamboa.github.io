## Listas e ciclos for
1.	melhor_fruta_do_mundo = frutas[1]
2.	começa a contar do fim
1.	LER COMENTÁRIOS - range tem intervalo exclusivo
```decrescente = range(9, 0, -1)
for numero in decrescente:
   print(numero)
```

3.	criar números pares + dois fors 
```
numeros_impares = range(1, 10, 2)
numeros_pares = range(2, 10, 2)
for numero in numeros_impares:
    print(numero)  
for numero in numeros_pares:
    print(numero)
```
### Aleatórios
1.	por geração do random dentro do for
2.	entre 0 e 1
3.	
```for i in range(1,10):
  alea = random()
  print(round(alea*5)+1 )
#–-OU--
for i in range(1,10):
    alea = random()
    print((round(alea*10) % 6) + 1)
```
### Donatello
1.	
```a = 100*2
b = 90
donatello.forward(a)
donatello.right(b)
donatello.forward(a)
donatello.right(b)
donatello.forward(a)
donatello.right(b)
donatello.forward(a)
```
2.	
```
for i in range(360):
   donatello.forward(1)
   donatello.right(1)
```
3.
```	
for i in range(360):
  donatello.forward(1)
  donatello.right(1)

for i in range(360):
  donatello.forward(1)
  donatello.left(1)
```
4.	
```for i in range(360*2):
   donatello.forward(1)
   donatello.right(1) if i <= 360 else donatello.left(1)
```
5.	 
```
for i in range(180):
  for i in range(360):
     donatello.forward(1)
     donatello.right(1) 
  donatello.right(10) 
```
