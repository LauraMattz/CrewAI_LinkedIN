
# CrewAI - Agentes de Post para LinkedIN 🤖

## Introdução 📚
Esse projeto utiliza **agentes inteligentes automatizados** para **criar posts para o LinkedIn** de maneira eficiente e escalável via ferramenta [CrewAI](https://www.crewai.com/).
- O objetivo é automatizar o processo de geração de posts otimizados, tornando a criação de conteúdo mais ágil e eficaz.

Este código foi projetado para rodar em **notebooks do Google Colaboratory**, aproveitando os recursos de computação em nuvem para realizar tarefas de scraping e geração de conteúdo.

## Funcionalidades 🎯
- **Agentes Inteligentes para Criação de Posts no LinkedIn**: Utilize agentes automatizados para gerar posts personalizados e de alta qualidade para o LinkedIn.
- **Automatização de Tarefas de Criação de Conteúdo**: Automatize as etapas de busca, redação e edição de posts.
- **Scraping de Dados**: Coleta de dados sobre tendências, tópicos populares e interações no LinkedIn e outros sites para melhorar o conteúdo gerado.
- **Integração com IA e ML**: Utilize tecnologias de inteligência artificial para gerar posts otimizados para o LinkedIn, adaptando o conteúdo para diferentes públicos e contextos.
- **Personalização e Otimização de Conteúdo**: Ajuste o conteúdo para que seja relevante para o público-alvo no LinkedIn, aumentando o engajamento.

## Fluxo de Trabalho 🛠️
O processo de criação de posts no LinkedIn é realizado por uma equipe de agentes, que executam as seguintes etapas:

1. **Buscador de Conteúdo**: O agente especializado em busca coleta dados relevantes sobre o tema desejado. Ele utiliza ferramentas de busca e scraping para extrair informações atualizadas e importantes da web.
2. **Redator de Conteúdo**: Após a coleta de dados, o agente redige posts para o LinkedIn, aproveitando as informações coletadas pelo agente de busca para criar conteúdo relevante.
3. **Editor de Conteúdo**: O agente editor revisa e ajusta o conteúdo gerado, garantindo que esteja bem estruturado e pronto para ser publicado no LinkedIn.

## Como Funciona 🤔
1. **Defina o Tema**: Escolha o tema ou assunto do post para o LinkedIn.
2. **Selecione os Agentes**: O sistema utiliza agentes especializados para buscar conteúdo, redigir e editar o post.
3. **Configure as Tarefas**: Defina as tarefas que os agentes realizarão (ex.: busca de conteúdo, redação, revisão, scraping).
4. **Execute a Equipe de Agentes**: Com um simples comando, a equipe de agentes começa a coletar dados e criar o conteúdo.
5. **Verifique o Resultado**: Analise o conteúdo gerado para garantir que ele esteja otimizado e pronto para ser publicado no LinkedIn.

Este projeto foi desenvolvido para ser executado no **Google Colaboratory**, aproveitando os recursos da nuvem para a execução de tarefas como scraping e processamento de conteúdo.

## Exemplo de Uso 📚

### Python
Aqui está um exemplo de como você pode utilizar o CrewAI para criar posts automatizados para o LinkedIn:

```python
from IPython.display import display, Markdown
import json

# Defina o tema do conteúdo
tema_do_post = 'CrewAI e um caso de escrita de post no Linkedin, como é esse caso'

# Crie um dicionário com as entradas necessárias para a equipe
entradas = {"tema": tema_do_post}

# Inicie a equipe e execute as tarefas com as entradas fornecidas
resultado = equipe.kickoff(inputs=entradas)

# Verifique se o resultado é um objeto JSON e, se for, converta para string em formato JSON
if isinstance(resultado, dict):
    resultado_str = json.dumps(resultado, indent=4)
else:
    resultado_str = str(resultado)

# Exiba o resultado em formato Markdown
display(Markdown(f"# Dados do Resultado

{resultado_str}"))
```

### Exemplo de Resultado 📊

Aqui está um exemplo de como o conteúdo gerado pode ser exibido:

```json
{🔍 Explorando a vanguarda da IA autônoma com a CrewAI 💡🚀

No mercado em rápida expansão de agentes de IA, a CrewAI emergiu como pioneira, garantindo um financiamento de $18 milhões e lançando uma plataforma inovadora de vários agentes para empresas gerenciarem autonomamente seus fluxos de trabalho complexos. 🚀📈

A CrewAI opera mais de 10 milhões de agentes mensalmente, com quase metade das empresas da Fortune 500 🏦✨ aproveitando sua estrutura open-source. E a recente estreia do CrewAI Enterprise, com adoção inicial de 150 clientes corporativos beta, promete simplificar o design, a implantação e o gerenciamento de agentes de AI para organizações de grande porte. 👥🔄⚙️

A plataforma multi-agente permite aos profissionais construir e implementar fluxos de trabalho automatizados usando qualquer modelo de linguagem grande (LLM) e plataforma em nuvem ☁️.

Os agentes da CrewAI são aplicáveis em uma ampla gama de setores, mostrando sua versatilidade:

👨‍💼 Planejamento Estratégico 💰 Finanças 📊 Métricas de Desempenho 🤖 Automação de IA 👩‍⚕️ Saúde 🧠 Aprendizado de Máquina 📈 Enriquecimento de Dados 📣 Marketing ☁️ Soluções em Nuvem 🔗 Integração de IA 📦 Cadeia de Suprimentos ⚙️ Automação de Tarefas 📚 Inteligência de Negócios 🎯 Posicionamento de Marca 💹 Otimização de Receita 🌱 Crescimento de Negócios 👩‍💼 Recursos Humanos

Para uma aprendizagem imersiva em sistemas multi-agentes, explore o curso 'Multi AI Agent Systems' de João Moura em colaboração com a DeepLearning.AI. Este curso, endossado por profissionais de IA, aplica o framework da CrewAI para decompor tarefas complexas para vários agentes de IA, aperfeiçoando técnicas como atuação, uso de ferramentas e colaboração entre agentes.

Não perca essa oportunidade de surfar a onda da IA, em direção a um ambiente de negócios mais colaborativo e eficiente. 🌊🤖💼

CrewAI #MultiAIAgents #DeepLearningAI #AI #MachineLearning #AIFunding.}
```

Este exemplo demonstra como o sistema gera conteúdo de forma automatizada, utilizando dados extraídos da web para criar posts otimizados para o LinkedIn.

## Requisitos 📝
- Python 3.6+ 🐍
- IPython 📊
- json 📈
- Biblioteca CrewAI 🤖
- **SerperDevTool** para buscas e scraping de dados 📡
- **ScrapeWebsiteTool** para raspagem de sites 🌐

## Instalação 📦
1. Instale o Python 3.6+ [aqui](https://www.python.org/downloads/).
2. Instale o IPython:
    ```bash
    pip install ipython
    ```
3. Instale a biblioteca `json` (geralmente já incluída com o Python):
    ```bash
    pip install json
    ```
4. Instale a biblioteca CrewAI:
    ```bash
    pip install crewai
    ```
5. Instale o pacote `crewai_tools` para buscar e raspar dados:
    ```bash
    pip install crewai_tools
    ```

## Contribuição 🤝
Se deseja contribuir para o projeto CrewAI, siga os passos abaixo:
1. Faça um fork do repositório 📁.
2. Crie uma nova branch para sua contribuição 📈.
3. Faça as alterações necessárias 📝.
4. Envie um pull request para o repositório principal 📈.

## Licença 📜
O projeto é licenciado sob a licença MIT. Você pode utilizar, modificar e distribuir o projeto de acordo com os termos dessa licença.

## Links úteis 🔗
- [Documentação do CrewAI](https://docs.crewai.com/introduction)
