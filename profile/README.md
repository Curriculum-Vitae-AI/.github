![Logo](https://github.com/user-attachments/assets/207da5fc-ba8e-411a-9c8c-1e3e48025f61)

# Time

| Nome                             |RA         |
| ---------------------------------| --------- |
| Bruno Costa Carvalho             | 821116933 |
| Erik Akio Matsumoto              | 821115561 |
| Gabriel Guardiano do Nascimento  | 821145633 |
| Gabriel Pastore                  | 821224010 |
| Mariana de Moraes Marcondes      | 821116771 |
| Renan Moura Silva                | 821145633 | 
| Vinícius Peralta                 | 821222997 |

# Curriculum AI

Curriculum AI é um projeto que tem como objetivo desenvolver uma interface gráfica com integração Gemini capaz de gerar roadmaps, cartas de motivação e indicar vagas conforme informações de experiência e vontades do usuário.

[Acesso a aplicação.](http://15.228.82.126/)

# Entregas

[Especificação do Projeto](EspecificacaoProjeto.pdf)

Abaixo estão os links da entregas conforme solicitado na Especificação do Projeto:

- [v0.0.1](https://github.com/Curriculum-Vitae-AI/Curriculum-AI-FrontEnd/releases/tag/v0.0.1);
- [v0.0.2](https://github.com/Curriculum-Vitae-AI/Curriculum-AI-FrontEnd/releases/tag/v0.0.2);
- [v1.0.0](https://github.com/Curriculum-Vitae-AI/Curriculum-AI-FrontEnd/releases/tag/v1.0.0);
- [v1.0.1](https://github.com/Curriculum-Vitae-AI/Curriculum-AI-BackEnd/releases/tag/v1.0.1);
- [v1.0.2](https://github.com/Curriculum-Vitae-AI/Curriculum-AI-BackEnd/releases/tag/v1.0.2);
- [v1.1.0](https://github.com/Curriculum-Vitae-AI/Curriculum-AI-BackEnd/releases/tag/v1.1.0);
- [v1.2.0](https://github.com/Curriculum-Vitae-AI/Curriculum-AI-BackEnd/releases/tag/v1.2.0);
- [v2.0.0](https://github.com/Curriculum-Vitae-AI/Curriculum-AI-FrontEnd/releases/tag/v2.0.0);

## Organização

Para organização do desenvolvimento criamos [Projetos](https://github.com/orgs/Curriculum-Vitae-AI/projects) onde para cada entrega temos um projeto que conta com um board definindo a estória a ser desenvolvida bem como as tarefas. Cada tarefa será linkada a uma branch e com isso é possivel acessar por meio da tarefa a sua Pull Request.

- [Entrega 01](https://github.com/orgs/Curriculum-Vitae-AI/projects/2);
- [Entrega 02](https://github.com/orgs/Curriculum-Vitae-AI/projects/4);
- [Entrega 03](https://github.com/orgs/Curriculum-Vitae-AI/projects/5);
- [Entrega 04](https://github.com/orgs/Curriculum-Vitae-AI/projects/6);
- [Entrega 05](https://github.com/orgs/Curriculum-Vitae-AI/projects/7/);
- [Entrega 06](https://github.com/orgs/Curriculum-Vitae-AI/projects/8/);
- [Entrega 07](https://github.com/orgs/Curriculum-Vitae-AI/projects/9/);
- [Entrega 08](https://github.com/orgs/Curriculum-Vitae-AI/projects/10/);

## Documentação

Abaixo segue documentação da aplicação:

- [API Back-End](https://curriculum-vitae-ai.github.io/Curriculum-AI-BackEnd/);

## Tecnologias

Para esta aplicação utilizaremos:

- [Node JS](https://nodejs.org/pt) (Back-End);
- [React JS](https://react.dev/) (Front-End);
- [Aiven.io](https://aiven.io/) (Banco de Dados);
- [AWS](https://aws.amazon.com) (Hospedagem Cloud);
- [PM2](https://pm2.keymetrics.io/) (Gerenciador de Processos - Back-End);
- [Nginx](https://nginx.org/) (Gerenciador de Processos - Front-End)

## Banco de Dados

Todas requisições realizadas ao Gemini são armazenadas em uma tabela registrando os seguintes dados:

- Requisição (JSON)
- Resposta (JSON)
- Serviço utilizado (ROADMAP, VAGAS ou CARTA_DE_MOTIVACAO)
- Data da requisição

![Tabela](https://github.com/user-attachments/assets/9867b6d0-9a79-42a9-95d3-06d26c9908cc)

## Deploy

Nossos deploys são realizados via [GitHub Actions](https://github.com/features/actions). Foi configurado nos repositórios de back-end e front-end arquivos de [workflow](https://github.com/Curriculum-Vitae-AI/Curriculum-AI-BackEnd/blob/main/.github/workflows/deploy-actions.yml) responsáveis por a cada vez que um merge for realizado na branch main iniciar o processo de deploy automático dependendo somente de uma aprovação de um dos administradores do repositório:

![](https://github.com/user-attachments/assets/4d30a01d-b33f-4d00-81dc-ab7c6cd2a1e6)

## Boas práticas

Para os repositórios desta organização temos alguns padrões a serem seguidos, segue lista:

- TODOS os commits devem seguir os padrões do [Conventional Commit](https://www.conventionalcommits.org/en/v1.0.0/), caso não sejam seguidos sua PR será automáticamente fechada;
- A branch _main_ é a principal de todos os repositórios, logo para commitar suas mudanças nela será necessário um Pull Request;
- O repositório [.github](https://github.com/Curriculum-Vitae-AI/.github) somente deve ser utilizado para atualizar a documentação da organização.
