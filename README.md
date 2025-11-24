# 🥈 Modelagem de Entidades com Abstração e Herança (Pessoa Física e Jurídica)

Este projeto demonstra a criação de uma hierarquia de classes em Java para modelar entidades com características comuns e específicas, aplicando os conceitos de **Classes Abstratas** e **Herança**.

---

## 🎯 Objetivo Principal

Criar uma estrutura de código que centralize atributos comuns (`nome`) em uma superclasse, enquanto delega a implementação de detalhes específicos (`cpf`, `cnpj`) para subclasses.

## 🛠️ Tecnologias e Conceitos de POO

* **Linguagem:** Java (Core)
* **Módulos/Conceitos:**
    * **Abstração:** Uso da `abstract class Pessoa` para definir um esqueleto que não pode ser instanciado diretamente.
    * **Herança:** `PessoaFisica` e `PessoaJuridica` **herdam** o atributo `nome` da classe `Pessoa` (Relação "É um").
    * **Encapsulamento:** Todos os atributos estão protegidos, com acesso via Getters e Setters.

## 🔑 Pontos de Destaque no Design

* **Centralização de Dados:** O atributo `nome` é definido uma única vez na classe `Pessoa`. Isso previne a duplicação de código e simplifica a manutenção, aderindo ao princípio **DRY** (Don't Repeat Yourself).
* **Conceito de Esqueleto:** A classe `Pessoa` é um esqueleto para tipos mais concretos. O sistema garante que ninguém instancie uma "Pessoa" genérica, apenas uma `PessoaFisica` ou `PessoaJuridica`.
