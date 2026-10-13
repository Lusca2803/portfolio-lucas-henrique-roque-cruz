# 💸 Sistema de Caixa e Cálculo de Troco
 
## 📝 Descrição do Projeto
Este projeto consiste em um algoritmo lógico para automação de frentes de caixa, focado no processamento de vendas e no cálculo otimizado de troco. O sistema gerencia desde a entrada do valor da compra até a decomposição do troco em cédulas de diferentes valores, garantindo que o cliente receba a menor quantidade possível de notas.
 
Desenvolvido como uma atividade de lógica de programação, o sistema utiliza estruturas de controle para validar pagamentos e realizar operações matemáticas de divisão inteira e resto (`div` e `mod`) para determinar a distribuição exata do dinheiro.
 

*Figura 1: Fluxograma completo do processo de venda e validação de pagamento.*
 
## 🚀 Funcionalidades Lógicas
O sistema é estruturado em módulos interdependentes:
* **Entrada e Validação:** Coleta o valor da compra e o valor pago, garantindo que o pagamento não seja inferior ao total (evitando "pagamento insuficiente").
* **Cálculo de Troco:** Operação aritmética simples para definir o valor total a ser devolvido ao cliente.
* **Decomposição de Cédulas:** Algoritmo que divide o valor do troco por notas de **R$ 100, 50, 20, 10, 5, 2 e 1**, atualizando o saldo restante a cada etapa.
* **Interface de Saída:** Exibição clara do resumo da transação e da lista detalhada de notas a serem entregues.
 
## 📊 Tecnologias e Conceitos Utilizados
* **Linguagem:** Pseudocódigo (Português Estruturado).
* **Conceitos de Programação:**
    * **Estruturas de Repetição:** Uso de `enquanto` para validação de entradas positivas.
    * **Estruturas Condicionais:** `se/entao/senao` para verificar a viabilidade do pagamento.
    * **Operadores Matemáticos:** Uso intensivo de `div` (quociente) e `mod` (resto) para contagem de cédulas.
 
## 🔧 Estrutura do Algoritmo
O projeto segue a seguinte sequência lógica baseada nos manuscritos:
1. **Obter valor_compra** e **valor_pago**.
2. **Validar Pagamento:** Se `valor_pago >= valor_compra`, prossegue; caso contrário, alerta erro.
3. **Calcular Troco:** `troco = valor_pago - valor_compra`.
4. **Decompor:**
   - `Notas100 = troco div 100`
   - `troco = troco mod 100`
   - (Repetir para 50, 20, 10, 5, 2 e 1).
5. **Exibir resultados.**
 

*Figura 2: Detalhamento do algoritmo de decomposição de notas.*
 
---
[Voltar ao início](https://github.com/Lusca2803/portfolio-lucas-henrique-roque-cruz)
