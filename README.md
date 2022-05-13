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
2) Alterar arquivo para que fique igual ao disponível nesse repositório.
3) [APENAS NA PRIMEIRA VEZ]
  - Vá nas configuracoes do VS Code clicando no ícone da engrenagem 
  - Clique no ícone no canto superior direito que transforma as configurações em código ("settings.json")
  - Adicione ao código:
  
    "editor.codeActionsOnSave": {
        "source.fixAll.eslint": true,
        "source.fixAll": true
    }
4) import React from 'react'; (Fazer importação no App.js para resolver erros)
