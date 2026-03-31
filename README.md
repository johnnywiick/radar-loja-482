# 🛡️ Radar Loja 482 — Sistema de Prevenção de Perdas

> O sistema que registra, monitora e documenta ocorrências de RFID violado em segundos.

![Status](https://img.shields.io/badge/Status-Em%20Produção-brightgreen)
![HTML](https://img.shields.io/badge/HTML-5-orange)
![JavaScript](https://img.shields.io/badge/JavaScript-ES6-yellow)
![Firebase](https://img.shields.io/badge/Firebase-Firestore-blue)

---

## 🚀 O que é o Radar Loja 482?

O **Radar Loja 482** é um sistema web de **Prevenção de Perdas** desenvolvido exclusivamente para a Loja 482, que permite o registro e monitoramento de ocorrências de **RFID violado** em tempo real.

O fiscal faz login com suas credenciais, registra a ocorrência com setor, SKU, valor e descrição — e o sistema armazena tudo com data/hora, gera relatórios filtrados por período e permite exportação em PDF.

---

## ✨ Funcionalidades

- 🔐 **Acesso restrito** com login por email e senha
- 📋 **Registro de ocorrências** com setor, código SKU, valor e descrição da peça
- 📍 **Seleção de localização** — Provador Feminino, Masculino, Salão de Vendas, Retaguarda ou Outros
- 📊 **Dashboard de resumo** com total de peças e prejuízo acumulado
- 🔍 **Filtro por período** com data inicial e final
- 📄 **Exportação em PDF** do relatório de ocorrências
- 🕒 **Registro automático** de data e hora de cada ocorrência
- 👤 **Identificação do fiscal** responsável em cada registro

---

## 🛠️ Tecnologias Utilizadas

| Tecnologia | Uso |
|---|---|
| **HTML5** | Estrutura da interface |
| **CSS3** | Estilização e responsividade |
| **JavaScript ES6** | Lógica e interatividade |
| **Firebase Firestore** | Banco de dados em tempo real |
| **Firebase Auth** | Autenticação de usuários |
| **jsPDF** | Exportação de relatórios em PDF |

---

## 💡 Como Funciona

```
1. Fiscal acessa o sistema com email e senha
        ↓
2. Seleciona o setor onde ocorreu a violação de RFID
        ↓
3. Informa o código SKU, valor e descrição da peça
        ↓
4. Registra a ocorrência com um clique
        ↓
5. Sistema salva com data, hora e nome do fiscal
        ↓
6. Dashboard atualiza total de peças e prejuízo em tempo real
        ↓
7. Gestor filtra ocorrências por período
        ↓
8. Exporta relatório completo em PDF
```

---

## 🔧 Como Rodar Localmente

### Pré-requisitos

- Navegador moderno (Chrome, Edge, Firefox)
- Conta no [Firebase](https://firebase.google.com) (para Firestore e Auth)

### Instalação

```bash
# Clone o repositório
git clone https://github.com/johnnywiick/radar-loja-482.git
cd radar-loja-482
```

### Configuração

Configure as credenciais do Firebase no arquivo `firebase-config.js`:

```js
const firebaseConfig = {
  apiKey: "sua_chave_aqui",
  authDomain: "seu_projeto.firebaseapp.com",
  projectId: "seu_projeto",
  storageBucket: "seu_projeto.appspot.com",
  messagingSenderId: "seu_id",
  appId: "seu_app_id"
};
```

### Executar

Abra o arquivo `index.html` diretamente no navegador ou sirva com um servidor local:

```bash
# Com Live Server (VS Code) ou qualquer servidor estático
open index.html
```

Acesse: `http://127.0.0.1:5500` *(ou conforme seu servidor local)*

---

## 🌐 Deploy em Produção

O projeto está hospedado no **GitHub Pages** com deploy automático via push na branch `main`.

🔗 URL de produção: [https://johnnywiick.github.io/radar-loja-482/](https://johnnywiick.github.io/radar-loja-482/)

---

## 📁 Estrutura do Projeto

```
radar-loja-482/
├── index.html          # Interface principal do sistema
├── style.css           # Estilização e tema visual
├── script.js           # Lógica de registro e relatórios
├── firebase-config.js  # Configuração do Firebase (não commitado)
└── .gitignore          # Arquivos ignorados pelo Git
```

---

## 🔒 Segurança

- Acesso restrito com autenticação obrigatória antes de qualquer registro
- Credenciais do Firebase protegidas via variáveis de ambiente
- Apenas fiscais cadastrados conseguem acessar o sistema
- Dados armazenados com segurança no Firestore

---

## 👨‍💻 Desenvolvedor

**Johnny Marcos**
Desenvolvido com 💙 usando HTML, JavaScript e Firebase.

[![GitHub](https://img.shields.io/badge/GitHub-johnnywiick-black?logo=github)](https://github.com/johnnywiick)

---

## 📄 Licença

Este projeto é proprietário. Todos os direitos reservados © 2026 Radar Loja 482.
