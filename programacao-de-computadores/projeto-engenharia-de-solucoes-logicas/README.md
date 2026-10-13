# 🏥 Saúde Pública: Sistema de Triagem Automatizada
 
## 📝 Descrição do Projeto
Este projeto consiste em um sistema de triagem inteligente desenvolvido para a priorização de atendimentos em unidades de emergência. O objetivo principal é automatizar a classificação de risco de pacientes através da análise de sinais vitais e sintomas, garantindo que casos críticos recebam atendimento imediato.
 
O algoritmo processa dados como **idade**, **batimentos cardíacos**, **temperatura** e **oxigenação** para determinar o nível de prioridade (Alta, Média ou Baixa). O sistema inclui uma etapa de validação rigorosa para evitar decisões baseadas em dados incorretos ou falhas nos sensores.
 
![WhatsApp Image 2026-03-26 at 22.02.54.jpeg](WhatsApp%20Image%202026-03-26%20at%2022.02.54.jpeg)
*Figura 1: Fluxograma do processo de triagem, da coleta de dados ao encaminhamento médico.*
 
## 🚀 Lógica do Sistema
O sistema opera seguindo um fluxo estruturado de decisão:
* **Coleta de Dados:** Entrada de informações do paciente e leitura de sensores (batimento, temperatura e oxigênio).
* **Validação de Segurança:** Verificação se os dados estão dentro de limites aceitáveis (ex: idade entre 0 e 120 anos) para evitar erros de digitação ou falhas técnicas.
* **Classificação de Risco:**
    * **Prioridade ALTA:** Batimento > 120 ou Temperatura > 39.0°C.
    * **Prioridade MÉDIA:** Batimento > 100 ou Temperatura > 37.5°C.
    * **Prioridade BAIXA:** Casos que não atingem os critérios de alerta acima.
* **Encaminhamento:** Registro no sistema, notificação da equipe médica e encaminhamento do paciente.
 
## 📊 Desafios e Aprendizados
* **Simplificação de Processos:** O maior desafio foi traduzir a complexidade de um atendimento real (que envolve múltiplos fatores) em decisões binárias e regras fixas para o algoritmo[cite: 1].
* **Integridade de Dados:** Implementação de loops de repetição (`enquanto`) para garantir que o processo só avance com dados válidos.
* **Saída de Dados:** Formatação de mensagens claras para o usuário final, como "Prioridade máxima - atendimento imediato".
 
![WhatsApp Image 2026-03-26 at 21.46.07.jpeg](WhatsApp%20Image%202026-03-26%20at%2021.46.07.jpeg)
*Figura 2: Implementação da lógica de classificação e resultados da triagem.*
 
## 🔧 Estrutura do Algoritmo
1. **Definição de Variáveis:** Uso de tipos `inteiro`, `real`, `cadeia` e `logico` para gerenciar as informações do paciente.
2. **Loop de Coleta:** Ciclo `enquanto (verdadeiro)` para entrada contínua de novos pacientes.
3. **Estrutura Condicional:** Uso de `se/entao/senao` aninhados para o cálculo preciso do nível de risco.
 
![WhatsApp Image 2026-03-26 at 21.46.00.jpeg](WhatsApp%20Image%202026-03-26%20at%2021.46.00.jpeg)
*Figura 3: Pseudocódigo da validação de dados e critérios de temperatura e batimento.*
 
---
[Voltar ao início](https://github.com/Lusca2803/portfolio-lucas-henrique-roque-cruz)
