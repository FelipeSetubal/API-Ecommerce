🛒 E-Commerce API with Flask

Uma API RESTful simples para simular funcionalidades básicas de um sistema de e-commerce, desenvolvida com **Python + Flask**. A aplicação permite o gerenciamento de produtos, autenticação de usuários, manipulação de carrinho e checkout, com persistência em banco de dados **SQLite**.

---

## 💡 Funcionalidades

- 🔐 Login e autenticação de usuários
- 🛍️ Adição, listagem, edição e exclusão de produtos
- 🛒 Adicionar/remover itens no carrinho
- 🧾 Visualizar itens do carrinho
- ✅ Realizar checkout
- 🔄 Suporte completo a métodos `POST`, `GET`, `PUT`, `DELETE`
- 🌐 Permissões de acesso com `@login_required`

---

## ⚙️ Tecnologias Utilizadas

- Python 3.12+
- Flask
- Flask-SQLAlchemy
- Flask-Login
- Flask-CORS
- SQLite

---

## 📁 Estrutura de Endpoints

### 🔐 Autenticação
| Método | Rota           | Descrição                  |
|--------|----------------|----------------------------|
| POST   | `/login`       | Login com username/senha   |
| POST   | `/logout`      | Logout do usuário logado   |

---

### 📦 Produtos
| Método | Rota                         | Descrição                      |
|--------|------------------------------|--------------------------------|
| POST   | `/api/products/add`          | Adicionar novo produto         |
| GET    | `/api/products`              | Listar todos os produtos       |
| GET    | `/api/products/<id>`         | Detalhar produto específico    |
| PUT    | `/api/products/update/<id>`  | Atualizar produto              |
| DELETE | `/api/products/delete/<id>`  | Deletar produto                |

---

### 🛒 Carrinho de Compras
| Método | Rota                           | Descrição                         |
|--------|--------------------------------|-----------------------------------|
| POST   | `/api/cart/add/<product_id>`   | Adicionar item ao carrinho        |
| DELETE | `/api/cart/remove/<product_id>`| Remover item do carrinho          |
| GET    | `/api/cart`                    | Visualizar itens no carrinho      |
| POST   | `/api/cart/checkout`           | Finalizar compra (limpa carrinho) |

---



