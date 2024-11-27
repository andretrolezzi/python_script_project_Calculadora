# Calculadora Simples em Python e Shell Script

Este repositório contém dois scripts para uma calculadora simples: um em **Python** e outro em **Shell Script**. Ambos os scripts permitem que o usuário faça operações matemáticas básicas, como soma, subtração, multiplicação e divisão.

## Como Executar o Arquivo `.sh`

O script Shell (`calculadora.sh`) permite que você execute a mesma calculadora diretamente no terminal em sistemas baseados em Unix (Linux, macOS). Para executá-lo, siga os passos abaixo:

### 1. **Dê Permissões de Execução ao Arquivo**

O arquivo `.sh` precisa de permissões de execução para ser executado no terminal. Para isso, siga este comando no terminal:

```bash
chmod +x calculadora.sh

Agora que o arquivo tem permissões de execução, você pode rodá-lo diretamente no terminal com o seguinte comando:
./calculadora.sh

O script pedirá para você inserir dois números e, em seguida, escolher uma operação entre soma, subtração, multiplicação e divisão. O resultado será mostrado na tela.

# Explicação do Código Python

Este script Python implementa uma calculadora simples que permite ao usuário realizar operações matemáticas básicas, como soma, subtração, multiplicação e divisão, entre dois números inseridos. A seguir, explicamos como o código funciona.

O script começa pedindo ao usuário para digitar dois números. Esses números são capturados como entradas de texto e convertidos para o tipo float para permitir cálculos com números decimais:
num1 = float(input("Digite o primeiro número: "))
num2 = float(input("Digite o segundo número: "))

Em seguida, o usuário é solicitado a escolher uma operação matemática entre soma, subtração, multiplicação ou divisão. A operação escolhida é capturada e armazenada na variável operacao:
operacao = input("Escolha a operação (+, -, *, /): ")

O script verifica qual operação foi escolhida e executa a operação correspondente:

Soma:
if operacao == '+':
    resultado = num1 + num2

Subtração:
elif operacao == '-':
    resultado = num1 - num2

Multiplicação:
elif operacao == '*':
    resultado = num1 * num2

Divisão:
elif operacao == '/':
    if num2 != 0:  # Verifica se não há divisão por zero
        resultado = num1 / num2
    else:
        print("Erro: Divisão por zero não é permitida.")
        exit(1)

Se o usuário escolher uma operação inválida, o script exibirá uma mensagem de erro e encerrará a execução:
else:
    print("Operação inválida.")
    exit(1)

4. Exibição do Resultado:
Por fim, o script exibe o resultado da operação realizada:
print(f"O resultado de {num1} {operacao} {num2} é: {resultado}")

























