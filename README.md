<p align="center">
  <a href="https://www.alura.com.br/" target="_blank">
    <img src="https://avatars.githubusercontent.com/u/4975968?s=200&amp" alt="Alura" width="150">
  </a>
</p>

# 🤖 Projeto Imersão 3 Alura iA Google Gemini:  Sistema de Pesquisa de Preços de Móveis e Produtos com Avaliação de Qualidade

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Gutobastos/imersao-iA-3-Alura/blob/main/projeto.ipynb)

Este projeto implementa um sistema avançado de pesquisa de preços para móveis e outros produtos, utilizando o poder de múltiplos agentes de Inteligência Artificial do Google Gemini. O objetivo é fornecer aos usuários informações detalhadas e avaliações de alta qualidade, otimizando o processo de compra.

## 🎯 Visão Geral

O sistema foi desenvolvido para simplificar a busca e seleção de produtos, oferecendo uma análise abrangente de custo-benefício, informações sobre a reputação dos vendedores e um resumo claro e organizado dos resultados. A arquitetura baseada em agentes permite que cada etapa do processo seja executada por um especialista em sua área.

## ✨ Funcionalidades

O sistema é composto por quatro agentes principais, cada um com um papel crucial:

1.  **🔍 Agente Buscador**:
    * Realiza a pesquisa inicial no Google, identificando produtos relevantes.
    * Filtra os resultados para garantir que apenas itens com preços sejam considerados.
    * Avalia fatores como garantia, reputação e avaliações dos vendedores.
    * Gera uma planilha detalhada de preços para facilitar a comparação.

2.  **💰 Agente Cotador**:
    * Atua como um filtro especializado, refinando os resultados da pesquisa inicial.
    * Foca em encontrar produtos com o melhor custo-benefício, priorizando os preços mais competitivos.
    * Seleciona de 1 a 5 produtos, fornecendo informações sobre preços e formas de pagamento disponíveis.

3.  **⭐ Agente Avaliador**:
    * Realiza uma avaliação de controle de qualidade dos produtos selecionados.
    * Prioriza produtos com as melhores médias de avaliações, utilizando o Google para obter dados precisos.
    * Inclui os preços na tabela de avaliação, oferecendo uma visão completa.
    * Gera um rascunho com os 5 produtos de melhor avaliação.

4.  **📢 Agente Retorno (Revisor)**:
    * Atua como um consultor de vendas, fornecendo informações completas e persuasivas sobre os produtos.
    * Especializado em vendas varejistas, com foco em custo-benefício e prazos de entrega.
    * Utiliza uma linguagem clara, respeitosa e confiante, adequada para um público entre 20 e 50 anos.
    * Revisa o rascunho do post, garantindo clareza, concisão, correção e o tom adequado.
    * Apresenta uma tabela com os 5 melhores produtos, ordenados por preço crescente, incluindo nome da empresa, avaliações positivas e hiperlinks diretos para os produtos.

## 🚀 Como Usar

1.  **Pré-requisitos**:
    * Certifique-se de ter a chave da API do Google configurada como uma variável de ambiente (`GOOGLE_API_KEY`).
    * As bibliotecas `google-genai` e `google-adk` devem estar instaladas no seu ambiente Python.

2.  **Instalação das Bibliotecas**:

    ```bash
    %pip -q install google-genai
    %pip -q install google-adk
    ```

3.  **Execução do Programa**:
    * Execute o script Python.
    * O programa solicitará que você digite o tipo de móvel ou produto que deseja pesquisar.
    * O sistema coordenará os agentes para realizar a busca, cotação, avaliação e geração do resultado final.
    * Os resultados serão exibidos no console, incluindo uma tabela detalhada com os produtos recomendados.
    * Para encerrar o programa, digite "sair", "SAIR" ou "Sair".

## 🗂️ Estrutura do Código

O código é organizado em funções que definem o comportamento de cada agente:

* `agente_buscador(topico, data_de_hoje)`: Implementa a lógica do Agente Buscador.
* `agente_cotador(topico, moveis_buscados)`: Implementa a lógica do Agente Cotador.
* `agente_avaliador(topico, avaliacao_de_post)`: Implementa a lógica do Agente Avaliador.
* `agente_retorno(topico, rascunho_gerado)`: Implementa a lógica do Agente Retorno (Revisor).
* Funções auxiliares como `call_agent()` para executar os agentes e `to_markdown()` para formatar a saída em Markdown.

## 🛠️ Tecnologias Utilizadas

* **<img src="https://www.python.org/static/img/python-logo.png" alt="Python" width="150"> Python**: A linguagem de programação principal utilizada no desenvolvimento.
* **<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/8/8a/Google_Gemini_logo.svg/344px-Google_Gemini_logo.svg.png" alt="Google Gemini" width="100"> Google Gemini**: Utilizado para os modelos de linguagem avançados.
* **Google ADK (Agent Development Kit)**: Framework para criação e gerenciamento dos agentes.
* **Google Search Tool**: Ferramenta para realizar pesquisas na web de forma eficiente.
* **<img src="https://avatars.githubusercontent.com/u/4975968?s=200&amp" alt="Alura" width="60"> Alura**: Plataforma de ensino que inspirou e contribuiu para o desenvolvimento deste projeto.
* **<img src="/img/vscodetransp.png" alt="Visual Studio Code" width="100"> Visual Studio Code**: Framework de desenvolvimento da Microsft.

## 🤝 Contribuição

<p align="center"><img src="https://avatars.githubusercontent.com/u/4975968?s=200&amp" alt="Alura" width="80"><img src="https://www.python.org/static/img/python-logo.png" alt="Python" width="250"><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/8/8a/Google_Gemini_logo.svg/344px-Google_Gemini_logo.svg.png" alt="Google Gemini" width="160"><img src="/img/vscodetransp.png" alt="Visual Studio Code" width="200"></p>


## 🧑‍💻 Autor
<img src="https://avatars.githubusercontent.com/u/168025112?v=4" alt="Alura" width="150">
<h4>Nome: Fabricio Augusto Oliveira Bastos</h2>
<h4>E-mail: mailto: "fabricio.bastos.ba@gmail.com" </h2>
