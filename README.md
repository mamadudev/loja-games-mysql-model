<div align="center">

# **Loja Games – Banco de Dados (MySQL)**

📦 Modelagem completa • 🧩 Relacionamentos • 🗄️ Script SQL pronto para uso

![Status](https://img.shields.io/badge/status-concluído-2ea44f)
![MySQL](https://img.shields.io/badge/MySQL-8.0-blue)
![Workbench](https://img.shields.io/badge/Workbench-Modelagem-orange)

</div>

---

## **📂 Acesso Rápido aos Arquivos**

* 📘 **Modelagem (Workbench)** → [db-schema.mwb](./db-schema.mwb)
* 🖼️ **Diagrama ER (PNG)** → [db-schema.png](./db-schema.png)
* 📄 **Diagrama ER (PDF)** → [db-schema.pdf](./db-schema.pdf)
* 💾 **Script SQL** → [db-schema.sql](./db-schema.sql)

---

## **📌 Sobre o Projeto**

Este repositório apresenta a modelagem de um banco de dados para uma loja de games.
Inclui o diagrama ER, script SQL completo e o arquivo editável criado no MySQL Workbench.

---

## **🧱 Estrutura das Tabelas**

### **tb_categorias**

* `id` (PK)
* `tipo`

### **tb_usuarios**

* `id` (PK)
* `usuario`
* `senha`
* `foto`
* `data_nascimento`

### **tb_produtos**

* `id` (PK)
* `nome`
* `descricao`
* `console`
* `quantidade`
* `preco`
* `foto`
* `categorias_id` (FK → tb_categorias.id)
* `usuarios_id` (FK → tb_usuarios.id)

---

## **🔗 Relacionamentos**

* Uma categoria pode ter vários produtos.
* Um usuário pode cadastrar vários produtos.

---

## **🛠️ Como usar**

### **Abrir o modelo**

Abra o arquivo:
`db-schema.mwb`

### **Criar o banco via script**

Execute no MySQL:

```sql
source db-schema.sql;
```

---

## **🚀 Possíveis melhorias**

* Adicionar dados de exemplo
* Criar views para consultas
* Integrar com uma API (Node.js)
* Expandir o modelo para clientes, pedidos e pagamentos

---

<div align="center">

Repositório organizado para estudo e prática de modelagem relacional.

</div>

