# 🍲🤖 Chatbot de Receitas com IA e AWS

<p align="center"><i>Um chatbot interativo que gera sugestões de receitas com base nos ingredientes que o usuário tem disponíveis. O sistema permite salvar receitas favoritas para consulta posterior.</i></p>

## 📖 Índice

1. [🏛️ Arquitetura](#-arquitetura-preliminar-aws)
2. [🛠️ Tecnologias Utilizadas](#-tecnologias-utilizadas)
3. [🚀 Execução e Utilização](#-execucao-e-utilizacao)
4. [🧱 Estrutura de Pastas](#-estrutura-de-pastas)
5. [🚧 Desafios e Dificuldades](#-desafios-e-dificuldades)
6. [👥 Contribuidores](#-contribuidores)

## 🌟 Objetivo

Desenvolver um chatbot capaz de sugerir receitas criativas com base nos ingredientes que o usuário possui. O chatbot também permitirá que os usuários salvem suas receitas favoritas para acesso futuro.

## 🏛️ Arquitetura Preliminar AWS

<p>A definir</p>

## 🛠️ Tecnologias Utilizadas
### 1. AWS Lex
Utilizado para criar o chatbot, permitindo a interação do usuário via texto dentro do Slack.

### 2. Amazon Bedrock
Usado para gerar receitas dinamicamente com base nos ingredientes inseridos pelo usuário, utilizando modelos de linguagem avançados.

### 3. AWS Lambda
Executa funções serverless para processar a lógica do chatbot, integrar o Bedrock e armazenar receitas favoritas.

### 4. Amazon DynamoDB
Banco de dados NoSQL para armazenar receitas favoritas e histórico de interação dos usuários.

### 5. Amazon API Gateway
Exponibiliza um endpoint seguro para receber requisições do Slack e encaminhá-las ao AWS Lambda.

### 6. AWS Secrets Manager
Armazena credenciais seguras para acessar a API do Slack e outros serviços sensíveis.

## 🚀 Execução e Utilização

### Fluxo do Chatbot
1. O usuário inicia uma conversa no Slack e informa os ingredientes que tem disponíveis.
2. O chatbot processa a entrada usando o **AWS Lex**.
3. O **AWS Lambda** recebe a informação e faz uma chamada ao **Amazon Bedrock** para gerar a receita.
4. A resposta com a receita é enviada de volta ao Slack.
5. O usuário pode optar por salvar a receita, armazenando-a no **DynamoDB**.

## 🧱 Estrutura de Pastas

```bash
/
|-- src/
|   |-- handlers/        # Funções AWS Lambda
|   |-- models/          # Estruturas de dados
|   |-- services/        # Integração com AWS
|-- assets/              # Imagens e documentos
|-- .env                 # Variáveis de ambiente
|-- README.md            # Documentação do projeto
```

## 🚧 Desafios e Dificuldades

- **Treinar a IA** para gerar receitas coerentes e variadas.
- **Integração segura com o Slack** garantindo autenticidade e segurança dos dados.
- **Otimização de latência**, garantindo respostas rápidas mesmo em picos de uso.

## 👥 Contribuidores

<table>
  <tr>
    <td align="center">
      <a href="https://github.com/DevDan7" title="GitHub">
        <img src="https://avatars.githubusercontent.com/u/152210372?v=4" width="100px;" alt="Foto Daniel"/><br>
        <sub>
          <b>Daniel Villegas</b>
        </sub>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/deboralopesdev" title="GitHub">
        <img src="https://avatars.githubusercontent.com/u/196735456?v=4" width="100px;" alt="Foto Debora"/><br>
        <sub>
          <b>Débora Lopes</b>
        </sub>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/oliviaoliva" title="GitHub">
        <img src="https://avatars.githubusercontent.com/u/89538707?v=4" width="100px;" alt="Foto Olivia"/><br>
        <sub>
          <b>Olivia Oliva</b>
        </sub>
      </a>
    </td>
  </tr>
</table>

---

📌 **Versão 1.0**

