# 🛡️ Algoritmo de Auditoria de Dados de Vendas
 ## 📝 Descrição do Projeto
Este projeto consiste em um sistema de monitoramento e auditoria para fluxos financeiros de vendas. O objetivo principal é automatizar a detecção de anomalias e garantir a integridade dos dados, identificando valores que fogem do padrão de segurança estabelecido.

O algoritmo processa entradas de vendas, calcula médias de desempenho e aplica filtros de quarentena. Ele foi projetado para atuar como uma camada de segurança inicial, exigindo intervenção manual (revisão do gerente) sempre que uma transação suspeita é detectada, permitindo inclusive o ajuste dinâmico dos parâmetros de segurança em tempo real.

*Figura 1: Fluxo lógico do sistema de auditoria e validação de limites.*

 ## 🚀 Funcionalidades e Regras de Negócio
O sistema opera baseado em três pilares de verificação:
* **Cálculo de Média:** Processamento da média aritmética de lotes de vendas para análise de volume.
* **Filtro de Quarentena:** Bloqueio automático do sistema caso a média das vendas ultrapasse o `LIMITE_SEGURANCA`.
* **Detecção de Discrepância:** Identificação de valores individuais que divergem drasticamente da média (outliers), sinalizando a necessidade de revisão manual.
* **Ajuste Dinâmico:** Interface via console que permite a um gestor validar vendas altas e atualizar o limite de segurança global durante a execução.

 ## 📊 Tecnologias Utilizadas
* **Linguagem:** Python 3.x
* **Ambiente de Desenvolvimento:** Google Colab / VS Code
* **Conceitos Aplicados:** Escopo de variáveis globais, estruturas condicionais avançadas, manipulação de tipos de dados (`float`, `string`) e entrada de dados dinâmica.

 ## 🔧 Como Executar
1. Certifique-se de ter o Python instalado em sua máquina.
2. Clone ou baixe o arquivo `projeto_algoritimo_de_alditoria_de_dados.py`.
3. Execute o script através do terminal:
   ```bash
   python projeto_algoritimo_de_alditoria_de_dados.py

[Voltar ao início](https://github.com/Lusca2803/portfolio-lucas-henrique-roque-cruz)
