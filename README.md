# IA-Assistente-de-Planejamento-de-Projetos-com-Agentes

Este projeto implementa um sistema de planejamento de projetos utilizando uma arquitetura baseada em múltiplos agentes de inteligência artificial (IA), construído com o Google Agent Development Kit (ADK) e o modelo Gemini da Google.

## Descrição

O sistema de planejamento de projetos é composto por uma série de agentes especializados, cada um responsável por uma etapa específica do processo de planejamento.  Estes agentes colaboram para coletar informações, definir objetivos, analisar restrições e gerar um plano de projeto completo.

Os agentes incluem:

*   **Agente de Contextualização:** Coleta informações sobre o contexto do projeto.
*   **Agente de Definição de Objetivos:** Define e prioriza os objetivos do projeto.
*   **Agente de Análise de Decisão:** Determina o tipo de decisão a ser tomada e os critérios de avaliação.
*   **Agente de Especificação de Detalhes:** Define o nível de detalhe necessário para o plano.
*   **Agente de Análise de Restrições:** Identifica e analisa as restrições do projeto.
*   **Agente de Coleta de Dados:** Identifica e coleta os dados relevantes para o planejamento.
*   **Agente de Tratamento de Dados:** Limpa, transforma e integra os dados coletados.
*   **Agente de Análise de Dados:** Realiza a análise dos dados para extrair insights.
*   **Agente de Avaliação de Alternativas:** Avalia diferentes alternativas de ação.
*   **Agente de Relatório:** Gera o relatório da proposta de planejamento.
*   **Agente de Formulário:** Cria o formulário de monitoramento de progresso.
*   **Agente de Apresentação:** Formata e apresenta os documentos de saída.

## Pré-requisitos

*   Conta Google com acesso à API Gemini.
*   Google Colab (recomendado para execução).
*   Chave da API Gemini configurada como um segredo no Google Colab (nomeado `GOOGLE_API_KEY`).
*   Pacote `google-adk` instalado.

## Instalação

1.  Clone este repositório para o seu ambiente local ou Google Colab.
2.  Instale o pacote `google-adk` utilizando o seguinte comando:

    ```bash
    !pip install -q google-adk
    ```
3.  Configure sua chave da API Gemini no Google Colab:

    *   Acesse a seção "Secrets" (ícone de chave) no painel esquerdo do Google Colab.
    *   Crie um novo segredo com o nome `GOOGLE_API_KEY` e cole sua chave da API Gemini como valor.

## Utilização

1.  Abra o notebook `ia_assistente_de_planejamento_de_projeto.py` no Google Colab.
2.  Execute as células do notebook em ordem.
3.  O sistema solicitará que você digite o tópico do projeto para o qual deseja criar um planejamento.
4.  Responda às perguntas dos agentes e forneça informações complementares quando necessário.
5.  O sistema irá iterar através dos diferentes agentes, gerando um plano de projeto passo a passo.

## Configuração

*   **Chave da API Gemini:** Certifique-se de configurar corretamente sua chave da API Gemini como um segredo no Google Colab.
*   **Modelo Gemini:** O código utiliza o modelo `gemini-2.0-flash`. Você pode modificar a variável `MODEL_ID` para usar um modelo diferente, se desejar.

## Licença

Este projeto está licenciado sob a [MIT License](LICENSE).

## Notas Adicionais

*   O código foi projetado para ser executado no Google Colab, mas pode ser adaptado para outros ambientes.
*   A qualidade do plano de projeto gerado depende da qualidade dos prompts e das informações fornecidas aos agentes.
