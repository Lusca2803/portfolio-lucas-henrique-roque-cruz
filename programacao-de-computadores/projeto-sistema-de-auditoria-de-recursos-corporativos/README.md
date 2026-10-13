# 🏢 Auditoria de Orçamentos Corporativos (Python)
 
[![Python Version](https://img.shields.io/badge/python-3.x-blue.svg)](https://www.python.org/)
[![Status](https://img.shields.io/badge/status-concluído-brightgreen.svg)]()
 
## 📖 Sobre o Projeto
Este projeto foi desenvolvido como parte da disciplina de Programação de Computadores do curso de Análise e Desenvolvimento de Sistemas. O objetivo do script é processar e calcular o orçamento de uma estrutura organizacional complexa (dicionários aninhados) de uma multinacional, aplicando regras de negócio dinâmicas e auditoria de execução.
 
A solução foi arquitetada utilizando conceitos avançados de Python para garantir flexibilidade, performance e rastreabilidade.
 
## 🚀 Funcionalidades
- **Cálculo Hierárquico:** Varredura completa da estrutura corporativa, independentemente do nível de profundidade.
- **Filtros Dinâmicos:** Capacidade de ignorar setores específicos e todos os seus subsetores na hora do cálculo financeiro.
- **Conversão de Câmbio:** Suporte a parâmetros opcionais para conversão de moedas em tempo de execução.
- **Sistema de Auditoria:** Monitoramento automatizado de tempo de execução e registro (logging) dos parâmetros utilizados na transação financeira.
 
## 🛠️ Tecnologias e Conceitos Aplicados
Este projeto foi construído utilizando Python puro (Standard Library), com foco nos seguintes paradigmas e recursos:
* **Funções Recursivas (Recursion):** Utilizadas para a navegação na árvore de dados (dicionários aninhados).
* **Decorators:** Implementação do `@auditor` para injetar comportamentos de log e cronometragem sem modificar a lógica de negócios.
* **Empacotamento de Argumentos (`*args` e `**kwargs`):** Utilizados tanto no decorator quanto na função principal para permitir a passagem dinâmica de departamentos a serem ignorados e taxas de câmbio.
 
## ⚙️ Como Executar
 
### Pré-requisitos
* Python 3.8 ou superior instalado.
 
### Passo a Passo
1. Clone este repositório:
   ```bash
   git clone (https://github.com/Lusca2803/projeto-sistema-de-auditoria-de-recursos-corporativos.git)
   ```
2. Acesse a pasta do projeto:
   ```bash
   cd projeto-sistema-de-auditoria-de-recursos-corporativos
   ```
3. Execute o script principal:
   ```bash
   python main.py
   ```
 
## 🧠 Lógica e Estrutura do Código
Breve explicação de como o código foi organizado:
* `Para construir a recursão, pensei na estrutura da empresa como uma árvore de departamentos, onde cada chave do dicionário poderia conter outro dicionário (subdepartamentos) ou um valor numérico representando o orçamento. A função percorre cada item verificando o tipo do valor: se for outro dicionário, ela chama a si mesma novamente para continuar navegando pela hierarquia; se for um número, o valor é somado ao total. Dessa forma, a solução funciona independentemente da profundidade da estrutura, tornando o algoritmo flexível para qualquer quantidade de níveis organizacionais.

O decorator foi acoplado ao projeto para adicionar uma camada de auditoria sem alterar a lógica principal da função de cálculo. Utilizei uma função wrapper que intercepta a execução da função original, registrando os argumentos recebidos, o início da auditoria e o tempo total de processamento usando a biblioteca time. O uso de *args e **kwargs dentro do decorator garantiu compatibilidade com qualquer parâmetro enviado para a função principal, mantendo o código reutilizável e organizado.`.
* **Dados:** Os dados simulados da empresa foram estruturados em... `A estrutura do dicionário foi organizada para representar a hierarquia de uma empresa de forma semelhante a uma árvore organizacional. Cada chave principal representa um setor ou unidade da empresa, como “Matriz” e “Filial_SP”. Dentro desses setores existem novos dicionários representando departamentos e subdepartamentos, permitindo criar níveis hierárquicos ilimitados. Os últimos níveis da estrutura, chamados de “folhas”, armazenam valores numéricos que representam os orçamentos de cada área específica.

Essa organização foi escolhida porque facilita o uso da recursão, já que a função consegue percorrer automaticamente todos os níveis do dicionário sem precisar conhecer previamente sua profundidade. Além disso, a estrutura aninhada torna o código mais próximo de cenários reais de empresas com múltiplos departamentos e subdivisões.`.
 
## 👤 Autor
 
* **Lucas Henrique Roque Cruz** * LinkedIn: https://www.linkedin.com/in/lucasroquecruz
* E-mail: lroque2803@gmail.com
 
---
*Projeto acadêmico com foco na aplicação prática de conceitos avançados da linguagem Python.*
