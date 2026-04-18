# Sistema Bancário em Python

Este projeto apresenta uma implementação de um sistema bancário simples em Python, desenvolvido como parte do desafio da Digital Innovation One (DIO). O objetivo é demonstrar conceitos de programação orientada a objetos (POO), modularização e boas práticas de desenvolvimento.

## Funcionalidades

O sistema bancário oferece as seguintes funcionalidades:

*   **Depósito**: Permite depositar valores em uma conta.
*   **Saque**: Permite sacar valores de uma conta, respeitando limites diários e de valor por saque.
*   **Extrato**: Exibe o histórico de transações (depósitos e saques) e o saldo atual da conta.
*   **Criação de Usuário**: Permite cadastrar novos usuários (Pessoa Física) com CPF, nome, data de nascimento e endereço.
*   **Criação de Conta Corrente**: Permite criar novas contas correntes vinculadas a um usuário existente, com agência e número de conta automáticos.
*   **Listagem de Contas**: Exibe todas as contas correntes cadastradas no sistema.

## Melhorias e Abordagem Orientada a Objetos

Esta versão do sistema bancário foi aprimorada a partir do desafio original da DIO, incorporando os seguintes princípios de Programação Orientada a Objetos (POO):

*   **Classes Abstratas (`ABC`)**: Utilização de classes abstratas para definir interfaces e garantir a implementação de métodos essenciais em subclasses, como `Transacao`.
*   **Herança**: Reutilização de código e especialização de classes, como `PessoaFisica` herdando de `Cliente` e `ContaCorrente` herdando de `Conta`.
*   **Encapsulamento**: Proteção de dados internos das classes através de atributos privados (`_`) e propriedades (`@property`).
*   **Polimorfismo**: Capacidade de objetos de diferentes classes responderem a uma mesma mensagem de forma diferente, como o método `sacar` em `Conta` e `ContaCorrente`.
*   **Modularização**: Organização do código em classes e funções bem definidas, facilitando a manutenção e a escalabilidade.

As principais classes implementadas são:

*   `Cliente`: Classe base para clientes, com métodos para realizar transações e adicionar contas.
*   `PessoaFisica`: Subclasse de `Cliente` para representar pessoas físicas, com atributos específicos como CPF.
*   `Conta`: Classe base para contas bancárias, com funcionalidades de depósito e saque.
*   `ContaCorrente`: Subclasse de `Conta` que adiciona limites de saque e número de saques diários.
*   `Historico`: Gerencia o histórico de transações de uma conta.
*   `Transacao`, `Saque`, `Deposito`: Classes abstratas e concretas para representar diferentes tipos de transações.

## Como Executar

Para executar o sistema bancário, siga os passos abaixo:

1.  **Salve o código**: Certifique-se de que o arquivo `sistema_bancario.py` está salvo em seu ambiente local.

2.  **Execute o script Python**:

    Abra um terminal ou prompt de comando, navegue até o diretório onde o arquivo `sistema_bancario.py` foi salvo e execute o seguinte comando:

    ```bash
    python3 sistema_bancario.py
    ```

    O programa será iniciado no terminal, apresentando um menu de opções para interagir com o sistema bancário.

## Estrutura do Projeto

```
. 
├── README.md
└── sistema_bancario.py
```

## Contribuição

Sinta-se à vontade para fazer um fork deste repositório, propor melhorias e contribuir com o projeto. Toda contribuição é bem-vinda!

## Autor

**Manus AI**

## Licença

Este projeto está licenciado sob a licença MIT. Veja o arquivo `LICENSE` para mais detalhes. (Nota: O arquivo LICENSE não está incluído neste exemplo, mas seria uma boa prática adicioná-lo.)
