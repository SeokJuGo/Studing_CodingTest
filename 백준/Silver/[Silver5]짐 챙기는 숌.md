# π‘ μ§ μ±κΈ°λ μ

| μκ° μ ν | λ©λͺ¨λ¦¬ μ ν | μ μΆ   | μ λ΅   | λ§ν μ¬λ | μ λ΅ λΉμ¨   |
| ----- | ------ | ---- | ---- | ----- | ------- |
| 2 μ΄   | 128 MB | 2542 | 1011 | 899   | 41.736% | 

## π λ¬Έμ 

μμ μ§μ μ±κ²¨μ κ²¨μΈμΊ νμμ μ§μΌλ‘ κ°λ €κ³  νλ€. κ·Όλ° μμ κ³΅λΆλ₯Ό λ§μ΄ νλ¬ μΊ νμ μ¨ κ²μ΄κΈ° λλ¬Έμ μ±μ μμ²­λκ² λ§μ΄ κ°μ§κ³  μλ€. μμ μ΄ μ±μ λ°©μ νμ²λΌ μμ λ¨λ€.

μμ μ±μ λ°μ€μ μ°¨κ³‘μ°¨κ³‘ λ£μ΄μ νλ°°λ‘ λ―Έλ¦¬ λ³΄λ΄λ €κ³  νλ€. μ±μ νμ²λΌ μ°¨κ³‘μ°¨κ³‘ μμ¬μκΈ° λλ¬Έμ, μ°¨λ‘λλ‘ λ°μ€μ λ£μ μλ°μ μλ€.

κ°κ°μ μ±μ λ¬΄κ²κ° μλ€. κ·Έλ¦¬κ³  λ°μ€λ μ΅λ λ£μμ μλ λ¬΄κ²κ° μλ€. μμ΄ νμν λ°μ€μ κ°μμ μ΅μκ°μ κ΅¬νλ νλ‘κ·Έλ¨μ μμ±νμμ€.

## μλ ₯

μ²«μ§Έ μ€μ μ±μ κ°μ Nκ³Ό λ°μ€μ λ£μ μ μλ μ΅λ λ¬΄κ² Mμ΄ μ£Όμ΄μ§λ€. Nμ 0λ³΄λ€ ν¬κ±°λ κ°κ³  50λ³΄λ€ μκ±°λ κ°μ μ μμ΄κ³ , Mμ 1,000λ³΄λ€ μκ±°λ κ°μ μμ°μμ΄λ€. Nμ΄ 0λ³΄λ€ ν° κ²½μ° λμ§Έ μ€μ μ±μ λ¬΄κ²κ° κ³΅λ°±μ μ¬μ΄μ λκ³  μ£Όμ΄μ§λ€. μ±μ λ¬΄κ²λ Mλ³΄λ€ μκ±°λ κ°μ μμ°μμ΄λ€.

## μΆλ ₯

μ²«μ§Έ μ€μ νμν λ°μ€μ κ°μμ μ΅μκ°μ μΆλ ₯νλ€.

### μμ  μλ ₯1

``` 
6 10
5 5 5 5 5 5
```

### μμ  μΆλ ₯1

``` 
3
```

## μμ  μλ ₯ 2

```
5 100
51 51 51 51 51
```

## μμ  μΆλ ₯ 2

```
5
```





### π Solution π

```
n,m=map(int,input().split())
count = 0
if n == 0 : print(0)
else : 
boxes = list(map(int,input().split()))
 weight = 0
 count = 1 
for box in boxes:  
 if box+weight <= m : 
weight += box
 else : 
weight = box 
count +=1
 print(count)
```
