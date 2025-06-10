# ❌ Não-as-a-Service

<p align="center">
  <img src="https://raw.githubusercontent.com/hotheadhacker/no-as-a-service/main/assets/imgs/naas-with-no-logo-bunny.png" width="800" alt="No-as-a-Service Banner" width="70%"/>
</p>

<p align="center">
  Este projeto é um fork do projeto original traduzido para o português (BR).<br>
</p>

Já precisou de uma maneira elegante de dizer "não"?
Esta pequena API retorna motivos de rejeição aleatórios, genéricos, criativos e, às vezes, hilários — perfeitamente adequados para qualquer cenário: pessoal, profissional, vida estudantil, vida de desenvolvedor ou simplesmente por diversão.

Criada para humanos, desculpas e humor.

## 🚀 Uso da API

**URL Base**
```
https://naas.isalman.dev/no
```

**Método:** `GET`  
**Limite:** `120 requisições por minuto por IP`

### 🔄 Exemplo de request
```http
GET /no
```

### ✅ Exemplo de Resposta
```json
{
  "razão": "Atualmente estou ocupado fingindo ser produtivo pela próxima década."
}
```

Use-o em aplicativos, bots, landing pages, integrações do Slack, cartas de rejeição ou onde quer que você precise de um não educado (ou espirituoso).

---

## 🛠️ Self-Hosting

Quer fazer você mesmo? É leve e simples.

### 1. Clone o repositório
```bash
git clone https://github.com/Woorkier/n-o-as-a-service.git
cd n-o-as-a-service
```

### 2. Instale as dependências
```bash
npm install
```

### 3. Inicie o servidor
```bash
npm start
```

A API estará disponível em:
```
http://localhost:3000/no
```

Você também pode trocar a porta ajustando a variável de ambiente:
```bash
PORT=5000 npm start
```

---

## 📁 Estrutura do Projeto

```
no-as-service/
├── index.js            # Express API
├── reasons.json        # 1000+ razões universais para dizer não
├── package.json
├── .devcontainer.json  # VS Code / Github devcontainer setup
└── README.md
```

---

## 📦 package.json

Para referência, aqui está a config do pacote (package.json):

```json
{
  "name": "no-as-service",
  "version": "1.0.0",
  "description": "Uma API leve que retorna rejeições aleatórias ou sem motivos.",
  "main": "index.js",
  "scripts": {
    "start": "node index.js"
  },
  "author": "hotheadhacker",
  "license": "MIT",
  "dependencies": {
    "express": "^4.18.2",
    "express-rate-limit": "^7.0.0"
  }
}
```

---

## ⚓ Devcontainer

Se você abrir este repositório no Github Codespaces, ele usará automaticamente `.devcontainer.json` para configurar seu ambiente. Se você abri-lo no VSCode, ele perguntará se você deseja reabri-lo em um contêiner.

---

> Quer usar o no-as-a-service no seu próprio projeto? Confira a seção de uso neste README e comece a retornar **"no"** como um profissional.
---

## 👤 Autor

Criado com teimosia criativa por [hotheadhacker](https://github.com/hotheadhacker)

---

## 📄 Licença

MIT — faça o que quiser, só não diga sim quando deveria dizer não.
