# Criando API com express

## Comandos básicos

Iniciar o npm (gerenciador de pacotes do node)
```
init -y
```

Instalar pacotes básicos
```
npm i express nodemon
```
* express: disponibiliza um ambiente de servidor
* nodemon: atualiza o servidor a cada edição dos arquivos

Criar arquivo para testar o servidor
```
touch server.js
```

Configurar o express no arquivo server.js criado
```
import express from 'express';
const app = express();

app.listen(3000, () => console.log(`Running at port 3000`));
```

Alterar script para rodar servidor
```
"start": "nodemon --exec server.js"
```
