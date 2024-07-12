# Plann.er API 💜

Projeto desenvolvido através do evento NLW - Journey, promovido pela Rocketseat.

Plann.er API é uma aplicação que permite fazer requisições através dos endpoints para interagir com o servidor e banco de dados, facilitando a gestão de viagens, participantes, atividades e links associados.

---

## Índice

1. [Sobre](#sobre)
2. [Endpoints](#endpoints)
    - [Trips](#trips)
    - [Participants](#participants)
    - [Activities](#activities)
    - [Links](#links)
3. [Tecnologias Utilizadas](#tecnologias-utilizadas)
4. [Instalação](#instalação)
5. [Uso](#uso)
6. [Contato](#contato)
7. [Agradecimentos](#agradecimentos)

---

## Sobre

Plann.er API é uma aplicação de backend que oferece uma série de endpoints para gerenciar viagens, participantes, atividades e links relacionados. O projeto foi desenvolvido durante o evento NLW - Journey promovido pela Rocketseat, e é um exemplo prático do uso de tecnologias modernas para construção de APIs.

## Endpoints

### Trips
- `GET /trips/{tripId}/confirm` - Confirma uma viagem.
- `POST /trips` - Cria uma nova viagem.
- `GET /trips/{tripId}` - Retorna os detalhes de uma viagem específica.
- `PUT /trips/{tripId}` - Atualiza as informações de uma viagem.

### Participants
- `PATCH /participants/{participantsId}/confirm` - Confirma a participação de um participante.
- `POST /trips/{tripId}/invites` - Envia convites para participar de uma viagem.
- `GET /trips/{tripId}/participants` - Lista os participantes de uma viagem.

### Activities
- `POST /trips/{tripId}/activities` - Adiciona uma nova atividade a uma viagem.
- `GET /trips/{tripId}/activities` - Lista as atividades de uma viagem.

### Links
- `POST /trips/{tripId}/links` - Adiciona um novo link a uma viagem.
- `GET /trips/{tripId}/links` - Lista os links de uma viagem.

---

## Tecnologias Utilizadas

<div>
  <img src="https://img.shields.io/badge/JavaScript-323330?style=for-the-badge&logo=javascript&logoColor=F7DF1E" alt="JavaScript"> 
  <img src="https://img.shields.io/badge/Node.js-43853D?style=for-the-badge&logo=node.js&logoColor=white" alt="Node.js"> 
  <img src="https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white" alt="TypeScript"> 
  <img src="https://img.shields.io/badge/SQLite-07405E?style=for-the-badge&logo=sqlite&logoColor=white" alt="SQLite"> 
  <img src="https://img.shields.io/badge/Prisma-3982CE?style=for-the-badge&logo=Prisma&logoColor=white" alt="Prisma"> 
</div>

---

## Instalação

Para configurar o ambiente e rodar o projeto localmente, siga os passos abaixo:

```bash
# Clone este repositório
git clone https://github.com/seu-usuario/plann-er-api.git

# Entre no diretório do projeto
cd plann-er-api

# Instale as dependências
npm install

# Configure o banco de dados (SQLite no exemplo)
npx prisma migrate dev

# Execute o projeto
npm start
```

---

## Uso

Para utilizar a API, siga os exemplos de endpoints fornecidos na seção [Endpoints](#endpoints). Você pode usar ferramentas como Postman ou Insomnia para testar as requisições.

```bash
# Exemplo de requisição para criar uma nova viagem
curl -X POST http://localhost:3000/trips -H "Content-Type: application/json" -d '{"name": "Viagem para a praia"}'
```

---

## Contato

Se você tiver alguma dúvida ou sugestão, sinta-se à vontade para entrar em contato através do email: fernandofagundes348@gmail.com.

---

## Agradecimentos

Agradeço à Rocketseat pelo evento NLW - Journey e ao professor Diego Fernandes pelo suporte e ensinamentos.

---
