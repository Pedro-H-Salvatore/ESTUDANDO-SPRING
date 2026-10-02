# 🌱 Evolução com o ecossistema Spring

Este repositório tem como objetivo registrar minha evolução no **ecossistema Spring**, por meio de estudos e projetos práticos.

As etapas serão atualizadas conforme meu avanço com o Spring e seus frameworks.

---

## 🗺️ Trilha de aprendizado

**Spring Web → Spring Data JPA → Spring Security**

| Etapa | Tecnologia | Status |
| :---: | --- | --- |
| 1 | Spring Web | Etapa inicial |
| 2 | Spring Data JPA | Próxima etapa |
| 3 | Spring Security | Etapa futura |

## 🚀 Etapa inicial — CRUD de marcas

O primeiro projeto será um **CRUD completo de marcas**, com as operações de:

- **Criação** de marcas;
- **Consulta** de marcas;
- **Atualização** dos dados de uma marca;
- **Exclusão** de marcas.

Nesta etapa, serão utilizados **Spring Web** e **Spring Boot DevTools**. O **Lombok** será usado para reduzir código repetitivo e facilitar o desenvolvimento.

## 🛠️ Tecnologias

| Tecnologia | Finalidade |
| --- | --- |
| Spring Web | Desenvolvimento da aplicação web e dos endpoints do CRUD |
| Spring Boot DevTools | Apoio ao desenvolvimento |
| Oracle Database | Armazenamento dos dados |
| Lombok | Redução de código repetitivo |

## 🗄️ Banco de dados

O projeto será configurado para o **Oracle**, utilizando o banco de dados disponibilizado pela minha instituição de ensino, a **FIAP**.

### Tabela de marcas

```sql
CREATE TABLE SPRING_MARCAS (
    ID_MARCAS NUMBER GENERATED ALWAYS AS IDENTITY,
    NOME      VARCHAR2(200) UNIQUE,
    TIPO      VARCHAR2(60) NOT NULL,
    FILIAIS   NUMBER NOT NULL
);
```

### Estrutura dos dados

| Campo | Tipo | Descrição |
| --- | --- | --- |
| `ID_MARCAS` | `NUMBER` | Identificador gerado automaticamente |
| `NOME` | `VARCHAR2(200)` | Nome da marca, com restrição de unicidade |
| `TIPO` | `VARCHAR2(60)` | Tipo da marca, com preenchimento obrigatório |
| `FILIAIS` | `NUMBER` | Quantidade de filiais, com preenchimento obrigatório |

## 📋 Regras de negócio

- Toda marca deve possuir um **identificador**, gerado automaticamente pelo banco.
- O **nome deve ser único** na tabela.
- O campo **tipo não pode ser nulo**.
- O campo **filiais não pode ser nulo**.

---

> 📚 Este repositório será atualizado ao longo dos estudos, acompanhando minha evolução e a incorporação de novas tecnologias do ecossistema Spring.
