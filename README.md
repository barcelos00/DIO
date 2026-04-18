# DIO
Sistema Bancário com Programação Orientada a Objetos em Python 🐍🏦

Este repositório contém a resolução do desafio de projeto da trilha de Python da Digital Innovation One (DIO). O objetivo foi evoluir um sistema bancário simples para uma estrutura robusta utilizando os pilares da Programação Orientada a Objetos (POO).

🚀 Objetivo do Projeto

Desenvolver um sistema bancário que permita a gestão de clientes e contas, realizando operações de depósito, saque e visualização de extrato, tudo isso aplicando conceitos avançados de Python para criar um código limpo, modular e escalável.

🛠️ Tecnologias Utilizadas

•
Python 3.x

•
Biblioteca textwrap: Para formatação de menus e strings.

•
Biblioteca datetime: Para registro temporal das transações.

•
Módulo abc: Para implementação de Classes Abstratas.

🏗️ Estrutura e Conceitos de POO Aplicados

Nesta versão, o sistema foi totalmente remodelado para seguir os princípios de POO:

•
Classes Abstratas (ABC): Implementadas na classe Transacao para garantir que diferentes tipos de movimentações (Saque/Depósito) sigam o mesmo contrato.

•
Herança:

•
PessoaFisica herda de Cliente.

•
ContaCorrente herda de Conta.



•
Encapsulamento: Uso de atributos privados (_saldo, _historico) e propriedades (@property) para proteger o estado dos objetos.

•
Polimorfismo: O método sacar é sobrescrito em ContaCorrente para incluir validações específicas de limites diários.

•
Composição: A classe Conta possui um Historico que armazena uma lista de objetos do tipo Transacao.

📋 Funcionalidades

1.
Gestão de Clientes: Cadastro de usuários (Pessoa Física) com CPF único.

2.
Gestão de Contas: Criação de múltiplas contas correntes vinculadas a um cliente.

3.
Operações Bancárias:

•
Depósito: Incrementa o saldo e registra no histórico.

•
Saque: Valida saldo, limite por saque e quantidade máxima de saques diários.

•
Extrato: Exibe detalhadamente todas as transações e o saldo atual.



📂 Como Executar

1.
Certifique-se de ter o Python instalado em sua máquina.

2.
Baixe o arquivo sistema_bancario.py.

3.
Execute o script via terminal:

Bash


python sistema_bancario.py





👤 Autor

Desenvolvido por Victor Santos Barcelos durante a trilha de Python da DIO, com o auxílio do Manus AI.




Este projeto faz parte do meu portfólio pessoal. Sinta-se à vontade para explorar, clonar e sugerir melhorias!

