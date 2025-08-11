# Documentação Base do Projeto

## Introdução

Para acessar a documentação dos repositórios acesse:

- [Backend](https://github.com/LucasSrSilva/anka-case-backend.git)
- [Frontend](https://github.com/LucasSrSilva/anka-case-frontend.git)

## Como iniciar o projeto

- Necessário docker instalado e rodando na máquina
- Faça o clone desse repositório

```bash
git clone https://github.com/LucasSrSilva/anka-case
```

- Acesse o repositório

```bash
cd anka-case
```

- Faça o clone dos próximos repositórios

```
git clone https://github.com/LucasSrSilva/anka-case-backend.git
git clone https://github.com/LucasSrSilva/anka-case-frontend.git
```

- Inicie o Docker Compose

```bash
docker compose up
```

- Acesse `http://localhost:3000` para vizualizar o frontend ou `http://localhost:3333/docs` para acessar a documentação

``

## Linha de Raciocínio Inicial

- A partir da leitura e análise das instruções do desafio técnico, optei por iniciar o desenvolvimento com foco na modelagem de dados, refletindo diretamente nas funcionalidades exigidas.

## Etapas e Estruturação

### 1. Modelagem de Dados

Com base nas funcionalidades obrigatórias, foi criado o arquivo de [modelagem de dados](./MODELAGEM_DADOS.md), contendo todos os modelos essenciais para:

- Clientes: dados pessoais, status e perfil familiar

- Metas financeiras: como aposentadoria ou objetivos de curto/médio prazo

- Carteira atual: classes e percentuais do patrimônio

- Projeções: crescimento patrimonial até 2060 com base em taxas personalizadas

- Histórico: registro de simulações

- Seguros: vida e invalidez

### 2. Estruturação do Backend

- Com os dados definidos, o próximo passo foi estruturar o backend, considerando as versões e tecnologias exigidas no case técnico, visto que o fastify 4 estava incompatível com zod4, resolvi continuar com fastify 5

- Gerado o crud inicial e a primeira formatação de dados, decidi iniciar o frontend
