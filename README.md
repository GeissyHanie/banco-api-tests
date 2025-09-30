# Banco API Tests

## 📌 Objetivo

Este projeto contém a automação de testes para a [Banco API](https://github.com/juliodelimas/banco-api).  
O propósito é validar os principais endpoints da API REST, contribuindo para a qualidade das operações.

---

## 🛠️ Stack Utilizada

- [Node.js](https://nodejs.org/)  
- [Mocha](https://mochajs.org/) – Framework de testes  
- [Chai](https://www.chaijs.com/) – Biblioteca de asserções  
- [Supertest](https://www.npmjs.com/package/supertest) – Testes de integração para APIs  
- [Mochawesome](https://www.npmjs.com/package/mochawesome) – Geração de relatórios em HTML  
- [dontenv](https://github.com/motdotla/dotenv) - Gerenciamento de variáveis de ambiente
- 
---

## 📂 Estrutura de Diretórios
```
banco-api-tests/
├── test/                 # Diretório com os arquivos de testes
│   ├── login.test.js     # Testes relacionados à autenticação
│   └── transferencias.test.js  # Testes relacionados a transferências
├── mochawesome-report/   # Relatórios HTML gerados após a execução
├── .env                  # Arquivo para configuração da variável BASE_URL
├── .gitignore          
├── package.json          
└── README.md             
```

---

## ⚙️ Arquivo `.env`
Este projeto necessita de um arquivo `.env` na raiz do projeto para definir a URL base da API.  
Exemplo:

```env
BASE_URL=http://localhost:3000
```

---

## ▶️ Execução dos Testes

1. **Instale as dependências:**
```bash
npm install
```

2. **Execute os testes:**
```bash
npm test
```

---

## 📊 Relatórios
Após rodar os testes, um relatório em HTML será gerado no diretório `mochawesome-report`.

Para abrir o relatório:
```bash
npx mochawesome-merge ./mochawesome-report/*.json > mochawesome.json
npx marge mochawesome.json
```

O arquivo final `mochawesome-report/mochawesome.html` poderá ser aberto diretamente no navegador.

---

## 📚 Documentações das Dependências
- [Mocha](https://mochajs.org/)  
- [Chai](https://www.chaijs.com/)  
- [Supertest](https://www.npmjs.com/package/supertest)  
- [Mochawesome](https://www.npmjs.com/package/mochawesome)  
- [dontenv](https://github.com/motdotla/dotenv)
---

✍️ Desenvolvido para apoiar a automação de testes da [Banco API](https://github.com/juliodelimas/banco-api).
