.. opus-udsl-docs documentation master file, created by
   sphinx-quickstart on Thu May  7 22:11:33 2020.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Welcome to Opus uDSL's documentation!
=====================================

.. toctree::
   :maxdepth: 2
   :caption: Contents:



Indices and tables
==================

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`

O que é o Opus uDSL Generator ?
===============================

É um gerador de código que tem como objetivo **acelerar o desenvolvimentos de sistemas com arquitetura baseada
em microserviços**.

Por que utilizar o uDSL Generator ?
===================================

* Simplifica e padroniza a geração de artefatos necessários para adoção da prática de "infraestrutura como código"
* Facilita o reuso de componentes e melhores práticas entre projetos  que adotam arquiteturas de microserviços
* Separação clara entre a definição da arquitetura de serviços de aplicação e componentes de suporte necessários
   para execução da aplicação em determinada plataforma

Features
========

* Permite descrever em alto nível uma aplicação baseada em microserviços por meio de 
  uma DSL (Domain-Specific Language)
* Uma mesma descrição de sistema pode ser reutilizada para diferentes plataforma-alvo, simplesmente
  alterando o arquivo de parametrização utilizado na geração
* Arquitetura extensível, permitindo a adição de novos módulos de geração voltados para novas plataformas-alvo
  de forma descritiva
* Geradores "out-of-the-box" disponíveis:
   * Terraform + Kubernetes: Gera artefatos Terraform para deploy da aplicação em um cluster Kubernetes padrão
   * Terraform + EC2: Gera artefatos Terraform para deploy da aplicação em instâncias EC2 da AWS.

Como usar o Opus uDSL Generator ?
=================================

1. :ref:`Descreva os macro-componentes de sua arquitetura utilizando a linguagem uDSL <udsl>`
2. :ref:`Crie o arquivo de parametrização para a plataforma desejada <config>` (EC2, K8S, etc)
3. :ref:`Execute o gerador, passando os arquivos contendo o modelo e parâmetros. <running>`
4. :ref:`Utilize os artefatos gerados para efetuar o deploy da aplicação na plataforma-alvo. <deploy>`

