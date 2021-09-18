## Sets

Set - Coleçcão de elementos
Definição - {Lista, de, elementos, dentro, de, um, frame}

Explícito
- Moeda {cara, coroa}
- Bits {0, 1}
- Dado {1, 2, 3, 4, 5, 6}

Implícito
- Dígitos {0, 1, ..., 9}
- Letras {a, b, ..., z}

Descritivo
- {palavra de 4 letras} = {casa, tema, hora, ...}


Sets comuns
- Inteiros {..., -2, -1, 0, 1, 2, ...} = Z
- Naturais {0, 1, 2, ...} = N
- Positivos {1, 2, 3, ...} = P
- Racionais {fração de inteiros m/n, n!=0} = Q
- Iracionais {não podem ser representados por uma fração, sqrt(2)}
- Reais = união entre Z, N, P, Q e I

Membros
- Elemento x está no set A; é um membro do set A; pertence ao set A -> 0 ∈ {0,1}, 1 ∈ {0,1}, 
- Não pertence -> 2 ∉ {0,1}

Sets especiais
- Vazio, não contém elementos -> ∅ ou {} -> ∀X, X∉∅ (∀ = Todos)
- Universal, contém todos os elementos -> Ω -> ∀∈Ω
    - Ω pode ser definido com um tipo, ex: Ω = R (números reais), Ω = {palavras}   

Python
```
# define um set {...} ou set({...})]
set1 = {1,2}
set2 = set({3,4})

# set vazio, apenas set({}), {} quando vazio é dict
setVazio = set({})
type(setVazio)
set

naoSetVazio = {}
type(naoSetVazio)
dict

# teste membros
1 in set1
True

5 in set1
False

5 not in set1
True

1 not in set1
False

# teste set vazio
S = set()
not S
True

T = {1,2}
not T
False

print(len(S)==0)
True

print(len(T)==0)
False
```

## Sets Simples

Sets de sets
- Sets definidos por um universo ou outro set
{x∈A | ...} = { elementos x em A do tipo ...} ou {x∈A:...}
Exemplo: N={x∈P|X>=0} ou P={x∈N|x>0}
-  Solução de equações  
{x∈R|x²>=0}} = R  
{x∈R|x²>=1}} = {-1,1}

Intervalos de inteiros
- {m,...n}={i∈Z}|m<=i<=n} intervalo de inteiros de m até n, incluso  
Exemplo:  
{3,...,5} = {i∈Z}|3<=i<=5} = {3,4,5}  
{3,...,4} = {i∈Z}|3<=i<=5} = {3,4}  
{3,...,3} = {i∈Z}|3<=i<=5} = {3}  
{3,...,2} = {i∈Z}|3<=i<=5} = ∅
- Conveção quando set inicia em 1: [n]={1,...,n}

- Intervalos Reais  
[] = pertence ao set, exemplo: [a,b] {x ∈ R | a <= x <= b} [3,5] = {3,4,5}  
() = não pertence ao set, exemplo: (a,b) {x ∈ R | a < x < b} (3,5) = {4}  
[a,b) = a incluso, b excluso [3,2]=[3,3)=(3,3]=∅

- Divisibilidade  
m,n ∈ Z  
Se n = c * m para algum c ∈ Zm dizemos que n é um múltiplo de m, ou m divide n, definimos com m|n. Exemplo:  
n=c*m = 6=2*3 = 3|6  
n=c*m = -8=(-2)*4 = 4|-8  
Quando n não é um múltiplo de m usamos ∤, exemplo:  
3∤4

Pyhton
```
# interalos e múltiplos {0,...n-1} similar a [n]={1..n}
print(set(range(3)))
{0,1,2}

# {m,...n-1}
print(set(range(2,5)))
{2,3,4}

# {m, m+d, m+2d, ...} < n-1
print(set(range(2,12,3)))
{8,2,11,5}
```

## Relações

