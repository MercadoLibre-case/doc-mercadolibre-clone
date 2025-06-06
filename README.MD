# 📘 Documentação – MercadoLibre Clone (Item Detail Page)

Este repositório contém toda a documentação técnica, arquitetural e organizacional do projeto **MercadoLibre Clone – Item Detail Page**, incluindo:

- Decisões técnicas
- APIs e contratos
- Instruções de execução
- Plano de testes
- Stack de tecnologias utilizadas

---

## 📂 Repositórios do projeto

| Repositório | Descrição |
|-------------|-----------|
| [`frontend-mercadolibre-clone`](https://github.com/MercadoLibre-case/frontend-mercadolibre-clone) | Interface Web do projeto, desenvolvida com Next.js, responsável por consumir os microserviços e renderizar a página de detalhe do produto |
| [`ms-product-detail`](https://github.com/MercadoLibre-case/ms-product-detail) | Microserviço responsável pelos dados do produto: título, descrição, imagens, preço, estoque e referência ao vendedor |
| [`ms-seller`](https://github.com/MercadoLibre-case/ms-seller) | Microserviço responsável por informações do vendedor, como nome da loja, reputação e total de vendas |
| [`ms-review`](https://github.com/MercadoLibre-case/ms-review) | Microserviço responsável por avaliações e notas dos produtos (ex: estrelas, número de reviews) |
| [`ms-payment-methods`](https://github.com/MercadoLibre-case/ms-payment-methods) | Microserviço responsável por fornecer os métodos de pagamento disponíveis para cada vendedor |
| [`doc-mercadolibre-clone`](https://github.com/MercadoLibre-case/doc-mercadolibre-clone) | Repositório de documentação técnica e arquitetural do projeto |

---


## 📌 Objetivo do projeto

Construir uma **página de detalhe de produto** inspirada no MercadoLibre, separando o frontend e os serviços backend em microserviços independentes, com comunicação via REST API.

---

## 📐 Arquitetura

- **Frontend**: Next.js (React)
- **Backend**: FastAPI (Python), dividido em microserviços
- **Persistência**: Arquivos JSON locais (sem banco de dados real)
- **Comunicação**: REST entre frontend e backend
- **Documentação**: Swagger/OpenAPI nos serviços + este repositório
- **Testes**: Cobertura mínima de 80% por serviço

---

## 🗂 Estrutura esperada

```bash
mercadolibre-clone/
├── doc-mercadolibre-clone/         📘 ← este repositório
├── frontend-mercadolibre-clone/    💻
├── ms-product-detail/              🔧
├── ms-review/                      ⭐️
└── ms-payment-methods/             💳