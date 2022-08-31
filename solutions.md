## Strings
1. 
```
nome='Jarvis'
print(nome)



print("Olá eu sou o " + nome)
print("Se estiver em apuros, chame" + nome)
print("Sim, o " + nome + " está sempre a sua doisposição")
```

## Inteiros, Floats e Calculadora
1. `print((a+b)*c)`
2.
```
d = (a+b)*c
print(d)
```
3.
```
e = 28820172 
print(e/1231)
```
4.
```
print(300/0)
# Resultado: ZeroDivisionError
```

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

## Aleatórios
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

## Booleanos
1. `aposta = True`
2. 
```
if e == aposta:
  print("Acertaste! Ganhaste 10 euros")
else:
  print("Falhaste! Perdeste 10 euros") 
```

## Donatello
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
## O Donatello quer ser um roomba
1.
```
for i in range(0, 3000):
  donatello.forward(1)
  posX, posY = donatello.pos()
  
  # rodar aleatóriamente entre -5 e 5 graus.
  a = round(random()*10)-5
  donatello.right(a)
```
2.
```
for i in range(0, 3000):
  donatello.forward(1)
  posX, posY = donatello.pos()
  
  # rodar aleatóriamente entre -5 e 5 graus.
  a = round(random()*10)-5
  donatello.right(a)

  # verificar se o donatelo sai do quadrado
  # entre (-100,-100) (100,100)
  if(posX <=- 100):
    donatello.right(40)
  if(posX >= 100):
    donatello.right(40)
  if(posY <= -100):
    donatello.right(40)
  if(posY >= 100):
    donatello.right(40)
```
## Cifrar como César
```
def encriptar(texto):
  res = ""
  for l in texto:
    n = chr(ord(l)+13)
    res += n
  return res
  
def desencriptar(texto):
  res = ""
  for l in texto:
    res+=chr(ord(l)-13)
  return res
  #one liner: "".join([chr(ord(i)-13)for i in texto])
```

## Fórmula Resolvente
```
delta = b**2 - 4*a*c # 0 está errado. colocar o valor certo.

if delta < 0:
  print("Não há raizes")
else:
  r1 = 0 # estes 0 também estão errados 
  r2 = 0 # idem
  print("As raizes são")
  print((-b + raiz_quadrada(delta))/(2*a))
  print((-b - raiz_quadrada(delta))/(2*a))
```
## Pi
```
for i in range(dardosTotal):
  # x e y deverão ser as coordenadas aleatórias de cada dado.
  x = random()
  y = random()
  
  x_ao_quadrado = x ** 2
  y_ao_quadrado = y**2 # Alterar
```
