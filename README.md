# 🔐 Página de Login & Cadastro

Projeto de uma tela de autenticação com animação de transição entre **Login** e **Cadastro**, desenvolvido como treinamento de HTML, CSS e JavaScript.

**Autor:** Rafael Sanguini Colagrossi

---

## 📁 Estrutura de arquivos

```
códigos/
├── index.html       # Estrutura da página
├── style.css        # Estilização completa
└── script.js        # Lógica de autenticação e validações
Imagens/
├── logo facebook.png    #foto da logo do facebook,não foi usada no projeto 
├── logo google.png      #foto da logo do google,não foi usada no projeto 
├── logo linkedin.png    #foto da logo do linkedin,não foi usada no projeto 
|
├ideias.md
└── README.md        # Este arquivo
```

---

## ✨ Funcionalidades

### Autenticação
- Cadastro de usuários com armazenamento em memória
- Login com validação de usuário e senha
- "Lembrar-me" via `sessionStorage`
- Redirecionamento para `home.html` após login bem-sucedido

### Validações
- Campos obrigatórios com feedback visual (borda vermelha/verde)
- Validação de formato de e-mail
- Mínimo de 3 caracteres para nome de usuário
- Mínimo de 6 caracteres para senha
- Confirmação de senha no cadastro
- Mensagens de erro específicas por campo

### Interface
- Animação de slide entre os painéis de Login e Cadastro
- Indicador de força da senha (Fraca → Muito Forte)
- Botão para mostrar/ocultar senha
- Toast notifications no lugar de `alert()`
- Modal de recuperação de senha (simulação)
- Placeholder some ao focar no campo
- Botões sociais: Google, Facebook, LinkedIn

---

## 🛠️ Tecnologias utilizadas

| Tecnologia | Uso |
|------------|-----|
| HTML5 | Estrutura semântica da página |
| CSS3 | Estilização, animações e responsividade |
| JavaScript (Vanilla) | Lógica de validação e interatividade |
| Google Fonts | Fontes *Playfair Display* e *DM Sans* |
| SVG inline | Ícones sem dependências externas |

---

## ⚙️ Como usar

1. Clone ou baixe os arquivos do projeto
2. Abra o `index.html` em qualquer navegador moderno
3. **Cadastre-se** primeiro para criar um usuário
4. Em seguida, faça **Login** com as credenciais criadas

> ⚠️ Os dados são armazenados apenas em memória — ao recarregar a página, os usuários cadastrados são perdidos. Para persistência real, integre com um backend ou substitua por `localStorage`.

---

## 📐 Estrutura do layout

```
┌─────────────────────────────────────┐
│  Painel Escuro  │   Formulário      │  ← Tela de Login
│  (bem-vindo)    │   (login)         │
├─────────────────────────────────────┤
│  Formulário     │   Painel Escuro   │  ← Tela de Cadastro
│  (cadastro)     │   (comunidade)    │
└─────────────────────────────────────┘
```

A troca entre as telas é feita via `<input type="checkbox" id="toggle">` + CSS puro, sem JavaScript para o slide.

---

## 🔮 Melhorias futuras

- [ ] Integração com backend (Node.js / PHP / Firebase)
- [ ] Hash de senha antes de armazenar
- [ ] Persistência real com banco de dados
- [ ] Autenticação via OAuth (Google, Facebook, LinkedIn)
- [ ] Recuperação de senha por e-mail
- [ ] Responsividade mobile aprimorada