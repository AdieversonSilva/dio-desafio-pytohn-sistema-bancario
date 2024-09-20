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

### 📝 Propostas de atualização do desafio

#### 1 📝 Otimizar o Sistema com Funções Python

Precisamos deixar nosso código mais modularizado, para isso vamos criar as funções para as operações existentes: sacar, depositar e visulizar extrato. Além disso, para a versão 2 do nosso sistema precisamos criar duas novas funções: criar usuário cliente banco) e criar conta corrente (vincular com usuário).

##### Funcções
Devemos criar funções para todas as operações do sistema. Para exercitar tudo o que aprendemos neste módulo, cada função vai ter uma regra na passagem de argumentos. O retorno e a forma como serão chamadas, pode ser definida por você da forma que acha melhor.

###### Saque 
A função saque deve receber os argumentos apenas por nome (keyword only). Sugestão de argumentos: saldo, valor, extrato, limite, numero_saques, limite_saques. Sugestão de retorno saldo e extrato.

###### Depósito
A função depósito deve receber os argumentos apenas por posição (posicional only). Sugestão de argumentos: saldo, valor, extrato. Sugestão de retorno: saldo e extrato.

###### Extrato
A função extrato deve receber os argumento por posição e nome (posicional only e keyword only). Argumentos posicionais: saldo, argumentos nomeados: extrato.

###### Novas funções
Precisamos criar duas novas funções: criar usuário e criar conta corrente. Fique a vontade para adicionar mais funções, exemplo: listar contas.

###### Criar usuário (cliente)
O programa deve armazenar os usuários em uma lista, um usuário é composto por: nome, data de nascimento, cpf e endereço. O endereço é uma string com o formato: logradouro, nro - bairro - cidade/sigla estado. Deve ser armazenado somente os números do CPF. Não podemos cadastrar 2 usuários com o mesmo CPF.

###### Criar conta corrente
O programa deve armazenar contas em uma lista, uma conta é composta por: agência, número da conta e usuário. O número de conta é sequencial, iniciando em 1. O número da agência é fixo: "0001". O usuário pode ter mais de uma conta, mas uma conta pertence a somente um usuário.

## 🔍 Referências

- [Digital Innovation One](https://www.dio.me/)
- [Documentação Git](https://git-scm.com/doc) 
- [Documentação Github](https://docs.github.com/)
- [Documentação Python](https://www.python.org/doc/)

<h5 align="center">
<img src="https://hermes.digitalinnovation.one/assets/diome/logo-full.svg" height="40" tittle="nome imagem"/> 

<hr>

![Static Badge](https://img.shields.io/badge/Git-f6522f?style=for-the-badge&logo=git&logoColor=000000) ![Static Badge](https://img.shields.io/badge/Github-c3c3c3?style=for-the-badge&logo=github&logoColor=000000) ![Static Badge](https://img.shields.io/badge/Python-fee469?style=for-the-badge&logo=python&logoColor=1c435f)