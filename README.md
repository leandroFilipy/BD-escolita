# 🏫 Sistema Escolar – Modelo Entidade-Relacionamento (MER)

Este projeto descreve o **Modelo Entidade-Relacionamento (MER)** de um sistema educacional básico, com foco na organização de turmas, salas e professores.

---

## 🔶 Diagrama ER

O modelo possui as seguintes entidades e relacionamentos:

### 📦 Entidades

- **TURMA**
  - Representa uma turma escolar.
  - Relaciona-se com `PROFESSORES` e `SALA`.

- **PROFESSORES**
  - Contém os dados dos professores da escola.
  - Relaciona-se com `TURMA` por meio do relacionamento `MINISTRA`.

- **SALA**
  - Representa as salas físicas da escola.
  - Relaciona-se com `TURMA` via o relacionamento `PERTENCEM`.

---

## 🔗 Relacionamentos

- **MINISTRA**
  - Relacionamento entre `PROFESSORES` e `TURMA`.
  - Um professor pode ministrar uma ou várias turmas.
  - Uma turma é ministrada por **um ou mais** professores.

- **PERTENCEM**
  - Relacionamento entre `TURMA` e `SALA`.
  - Uma turma pertence a uma sala.
  - Uma sala pode ter várias turmas ao longo do tempo (ex: horários diferentes).

---

## 💡 Exemplo de Interpretação

- O professor João ministra a Turma A.
- A Turma A pertence à Sala 101.
- A Sala 101 pode ser usada por outras turmas em diferentes horários.

---

## 📄 Licença

Este material é livre para fins acadêmicos e educacionais. Licenciado sob a [MIT License](LICENSE).

---

## ✍️ Autor

Diagrama criado como parte do estudo de modelagem de dados para sistemas educacionais.

---
