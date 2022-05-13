# Configuração de arquivos para o ambiente React.Js
Minhas configurações personalizadas e como aplicá-las.

Vamos configurar os seguintes arquivos:
- .prettierrc.js (Prettier)
- .editorconfig (Editorconfig)
- .eslintrc.js (Eslint)

OBS: Antes de tudo as extensões devem estar instaladas no Visual Studio Code:
[imagens aqui]

## Editorconfig
1) Com a extensão instalada basta clicar com o botão direto do mouse na pasta atual (pelo VS code mesmo) e selecionar a nova opção disponível "generate .editorconfig". 
2) Alterar arquivo para que fique igual ao disponível nesse repositório.

## Prettier
1) Adicionar manualmente o arquivo .prettierrc.js 
2) Alterar arquivo para que fique igual ao disponível nesse repositório.

## Eslint
1) $ npx eslint --init
2) [APENAS NA PRIMEIRA VEZ]
  - Vá nas configuracoes do VS Code clicando no ícone da engrenagem 
  - Clique no ícone no canto superior direito que transforma as configurações em código ("settings.json")
  - Adicione ao código:
  
    "editor.codeActionsOnSave": {
        "source.fixAll.eslint": true,
        "source.fixAll": true
    }
3) import React from 'react'; (Fazer importação no App.js para resolver erros)
4) $ npm i -D prettier eslint-config-prettier eslint-plugin-prettier
5) Adicionar em .eslintrc.js dentro do grupo "env" a linha:

    "jest": true,
    
6) Verificar se tudo está rodando corretamente em Terminal>Saída>ESLint

OBS: O ideal é fazer essas configurações no início de um projeto, mas, se já for um projeto em andamento, faça o seguinte para aplicar correções:

$ npx eslint src/**/*.jsx --fix

$ npx eslint src/**/*.js --fix

## Extra: Prop Types

Aproveite o clima de configurações e já deixe o prop types instalado com:

$ npm i prop-types

OBS: Na hora de usar lembre-se de importar a biblioteca:

import P from 'prop-types'
