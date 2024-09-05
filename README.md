<h1 align="center">
<img src="https://hermes.dio.me/tracks/2a3a2d2b-7de7-457c-b4df-dcd327eae9eb.png" height="150" tittle="Engenharia de Dados - NTT Data"/>
</h1>
<h2 align="center">
Desafio - Criando um sistema Bancário com Python
</h2>

### 📝 Proposta do repositório

Repositório para armazenar arquivos do desafio proposto pela [Digital Innovation One](https://www.dio.me/), no Bootcamp <strong>Engenhraria de Dados - NTT Data. </strong>

### 📝 Proposta do desafio

Criar sistema bancário com as operações: sacar, depositar e visualizar extrato.

Fomos contratados por um grande banco para desenvolver o seu novo sistema. Esse banco deseja modernizar suas operações e para isso escolheu a linguagem Python. Para a primeira versão do sistema devemos implementar apenas 3 operações: <strong> depósito, saque e extrato.</strong>

##### Operação de depósito
<p> Deve ser possível depositar valores positivos para a minha conta bancária. A v1 do projeto trabalha apenas com 1 usuário, dessa forma não precisamos nos preocupar em identificar qual é o número da agência e conta bancária. Todos os depósitos deve ser armazenados em uma variável e exibidos na operação de extrato. </p>

##### Operação de saque
<p>
O sistema deve permitir realizar 3 saques diários com limite máximo de R$ 500,00 por saque. Caso o usuário não tenha saldo na conta, o sistema deve exibir uma mensagem informando que não será possível sacar o dinheiro por falta de saldo. Todos os saques devem ser armazenados em uma variável e exibidos na operação de extrato.
</p>

##### Operação de extrato
<p>
Essa operação deve listar todos os depósitos e saques realizados na conta. No fim da listagem deve ser exibido o saldo atual da conta.
</p>
<p>
Os valores devem ser exibidos utilizando o formato R$ xxx.xx, exemplo: <br>
    1500.45 = R$ 1500.45
</p>

### 📜 Scripts Modelos
``` 
menu = """

[d] Depositar
[s] Sacar
[e] Extrato
[q] Sair

=> """

saldo = 0
limite = 500
extrato = ""
numero_saques = 0
LIMITE_SAQUES = 3

while True:

    opcao = input(menu)

    if opcao == "d":
        print("Depósito")

    elif opcao == "s":
        print("Sacar")

    elif opcao == "e":
        print("Extrato")
        
    elif opcao == "q":
        break

    else:
        print("Operação inválida, por favor selecione novamente a operação desejada.")
```

## 🔍 Referências

- [Digital Innovation One](https://www.dio.me/)
- [Documentação Git](https://git-scm.com/doc) 
- [Documentação Github](https://docs.github.com/)
- [Documentação Python](https://www.python.org/doc/)

<h5 align="center">
<img src="https://hermes.digitalinnovation.one/assets/diome/logo-full.svg" height="40" tittle="nome imagem"/> 

<hr>

![Static Badge](https://img.shields.io/badge/Git-f6522f?style=for-the-badge&logo=git&logoColor=000000) ![Static Badge](https://img.shields.io/badge/Github-c3c3c3?style=for-the-badge&logo=github&logoColor=000000) ![Static Badge](https://img.shields.io/badge/Python-fee469?style=for-the-badge&logo=python&logoColor=1c435f)