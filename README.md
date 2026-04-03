# Módulo 2 / 🐍 baseado no curso Santander + Cursor

*concluí o [modulo-01](https://github.com/Aldertvdev/Modulo-1-Phyton-IA/blob/main/README.md)*, vamos no módulo 2:🧑🏻‍🏫

- 1 Introdução ao Cursor (conceitos)
O que é Cursor (VS Code + IA)
Como instalar (no computador)
Configurar modelo de IA (Claude 3.5 Sonnet, GPT-4o, etc.)
Interface principal: sidebar, chat, composer
- 2 Principais funcionalidades da IA no Cursor
Chat lateral (perguntar sobre código)
Cmd/Ctrl + K → gerar ou editar código
Composer (Ctrl + I) → criar arquivos ou features inteiras com IA
Auto-complete inteligente (tab para aceitar sugestão)
Debug com IA
- 3 Fluxo de trabalho com Python + IA
Criar scripts mais avançados
Usar bibliotecas (ex: pandas, requests – mas no Pydroid 3 algumas não funcionam bem)
Refatorar código (melhorar código ruim)
Gerar funções, classes básicas
- 4 Exemplos práticos comuns no Módulo 2

# Exemplo 1: Funções básicas (muito usado com IA

```cpp
print("=== Módulo 2 - Funções ===\n")

def saudacao(nome):
    return f"Olá {nome}! Bem-vindo ao curso de Python com IA."

def calcular_media(notas):
    return sum(notas) / len(notas)

# Usando as funções
print(saudacao("Yuri Gabriel"))

notas_aluno = [8.5, 7.0, 9.5, 6.0]
media = calcular_media(notas_aluno)
print(f"Sua média é: {media:.2f}")

if media >= 7:
    print("Aprovado!")
else:
    print("Precisa estudar mais.")
```
exibirá:

```cpp
=== Módulo 2 - Funções ===

Olá Yuri Gabriel! Bem-vindo ao curso de Python com IA.
Sua média é: 7.75
Aprovado!
```

# Exemplo 2: Listas + dicionários + if (nível intermediário)

```cpp
print("=== Exemplo Módulo 2 - Gerenciador simples ===\n")

alunos = {
    "Yuri": {"idade": 17, "nota": 8.5},
    "Ana": {"idade": 19, "nota": 9.0},
    "João": {"idade": 16, "nota": 5.5}
}

for nome, dados in alunos.items():
    status = "Aprovado" if dados["nota"] >= 7 else "Recuperação/Reprovado"
    print(f"Aluno: {nome} | Idade: {dados['idade']} | Nota: {dados['nota']} → {status}")
```

exibira: 

```cpp
=== Exemplo Módulo 2 - Gerenciador simples ===

Aluno: Yuri | Idade: 17 | Nota: 8.5 → Aprovado
Aluno: Ana | Idade: 19 | Nota: 9.0 → Aprovado
Aluno: João | Idade: 16 | Nota: 5.5 → Recuperação/Reprovado

[Program finished]
```

# Exemplo 3: Input + loop + condicional (projeto pequeno)

```cpp
print("=== Calculadora simples (estilo Módulo 2) ===\n")

def calculadora():
    num1 = float(input("Digite o primeiro número: "))
    operacao = input("Digite a operação (+, -, *, /): ")
    num2 = float(input("Digite o segundo número: "))

    if operacao == "+":
        resultado = num1 + num2
    elif operacao == "-":
        resultado = num1 - num2
    elif operacao == "*":
        resultado = num1 * num2
    elif operacao == "/":
        resultado = num1 / num2 if num2 != 0 else "Erro: divisão por zero"
    else:
        resultado = "Operação inválida"

    print(f"Resultado: {resultado}")

calculadora()
```
exibirá:
```cpp
print("=== Calculadora simples (estilo Módulo 2) ===\n")

def calculadora():
    num1 = 17.0          # número fixo
    operacao = "+"       # operação fixa
    num2 = 6.0           # número fixo

    if operacao == "+":
        resultado = num1 + num2
    elif operacao == "-":
        resultado = num1 - num2
    elif operacao == "*":
        resultado = num1 * num2
    elif operacao == "/":
        resultado = num1 / num2 if num2 != 0 else "Erro: divisão por zero"
    else:
        resultado = "Operação inválida"

    print(f"Resultado: {resultado}")

calculadora()
```
Gostou? volte no [Curso inteligente com IA](https://github.com/Aldertvdev/Curso-Python-com-IA)
