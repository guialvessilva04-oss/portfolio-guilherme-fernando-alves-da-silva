# 🤖 Batalha de Modelos & Engenharia de Prompt (XML)

## 📝 Descrição do Projeto
[cite_start]Este projeto consiste em um estudo comparativo de performance entre diferentes Large Language Models (LLMs) através da aplicação de **Engenharia de Prompt Estruturado em XML**[cite: 60, 63]. [cite_start]O objetivo central foi criar um prompt robusto e técnico para a geração automática de uma página HTML *Single Page* com CSS integrado, testando a capacidade de compreensão estrutural de diversas IAs de ponta[cite: 62, 63].

[cite_start]Desenvolvido pelos alunos **Guilherme Fernando Alves da Silva** e **Klener Nilmar**, o experimento utilizou um protocolo de execução rigoroso para avaliar como cada modelo interpreta diretrizes de design, layout responsivo e métricas de consumo de tokens[cite: 60, 65].

## 🚀 Tecnologias e Ferramentas Testadas
[cite_start]O prompt estruturado foi submetido a um teste de estresse nos seguintes modelos[cite: 63, 67]:
* **Principais competidores:** DeepSeek, Claude, ChatGPT (GPT), Gemini.
* **Outras ferramentas:** Qwen, Grok e Maritaca.
* [cite_start]**Técnica de Prompting:** Estruturação hierárquica via tags XML (`<tarefa>`, `<diretrizes_design>`, `<obrigatoriedades_tecnicas>`).

## 📊 Quadro de Análise Comparativa
[cite_start]Os modelos foram avaliados em critérios de precisão técnica e criatividade[cite: 66, 67]:

| Critérios de Avaliação | GPT | Gemini | DeepSeek | Claude | Qwen | Grok | Maritaca |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| **Precisão do HTML** | [cite_start]7.3 [cite: 67] | [cite_start]8.0 [cite: 67] | [cite_start]9.0 [cite: 67] | [cite_start]7.5 [cite: 67] | [cite_start]7.6 [cite: 67] | [cite_start]7.7 [cite: 67] | [cite_start]7.3 [cite: 67] |
| **Criatividade** | [cite_start]4.0 [cite: 67] | [cite_start]5.0 [cite: 67] | [cite_start]9.5 [cite: 67] | [cite_start]7.5 [cite: 67] | [cite_start]7.4 [cite: 67] | [cite_start]7.3 [cite: 67] | [cite_start]4.5 [cite: 67] |
| **Tokens Gerados** | [cite_start]~1000 [cite: 67] | [cite_start]1350 [cite: 67] | [cite_start]~2450 [cite: 67] | [cite_start]~5000 [cite: 67] | [cite_start]3200 [cite: 67] | [cite_start]1240 [cite: 67] | [cite_start]1250 [cite: 67] |

## 🧠 Resultados e Aprendizados
A experiência revelou dados valiosos sobre a eficiência dos modelos atuais:
* [cite_start]**Liderança em Compreensão:** O **DeepSeek** demonstrou a maior "compreensão" da estrutura XML, entregando o resultado mais criativo e preciso[cite: 69].
* [cite_start]**Eficiência de Tokens:** Observou-se que uma maior quantidade de tokens (como no caso do Claude) não garante necessariamente um resultado superior; o DeepSeek foi mais eficiente na relação entre custo (tokens) e benefício (qualidade)[cite: 70].
* [cite_start]**Recomendação de Uso:** Com base nos testes, o **DeepSeek** é a escolha ideal para prototipagem rápida, enquanto o **Claude** é recomendado para códigos de alta complexidade[cite: 71].
* [cite_start]**Confiabilidade:** Todos os modelos testados apresentaram **zero erros de sintaxe (bugs)** no código gerado[cite: 67].

## 🔧 Estrutura do Prompt Utilizado
O esqueleto do prompt XML seguido foi:
```xml
<tarefa>
    <objetivo>Criar uma página HTML5 única com CSS3 interno.</objetivo>
    <diretrizes_design>
        <layout>Responsivo e minimalista.</layout>
        <tipografia>Sans-serif para títulos, Serif para corpo.</tipografia>
    </diretrizes_design>
    <obrigatoriedades_tecnicas>
        <item>Menu de navegação funcional (âncoras).</item>
        <item>Seção de portfólio ou galeria.</item>
    </obrigatoriedades_tecnicas>
</tarefa>
