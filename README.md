# Gulp com Sass

Este é um projeto simples que utiliza o Gulp para automatizar a transformação e otimização de arquivos Sass para CSS, além de copiar um arquivo HTML de origem para um diretório de destino.

## Estrutura do Projeto

|-- src/
| |-- sass/
| | |-- index.scss
| |-- index.html
|-- build/
| |-- css/
| | |-- estilo.min.css
|-- gulpfile.js
|-- package.json


- **src/**: Contém os arquivos de origem.
  - **sass/**: Armazena o arquivo Sass principal (`index.scss`) e outros arquivos relacionados ao estilo.
  - **index.html**: O arquivo HTML principal do projeto.

- **build/**: Diretório de destino para os arquivos processados.
  - **css/**: O CSS otimizado gerado pelo Gulp.

- **gulpfile.js**: Configurações e tarefas do Gulp.

- **package.json**: Informações sobre o projeto e suas dependências.

## Tarefas do Gulp

1. **Transformação de CSS com Sass:**
   - A tarefa `transformacaoCSS` converte o arquivo Sass principal (`src/sass/index.scss`) em um arquivo CSS otimizado (`build/css/estilo.min.css`).
   - Isso envolve a compilação Sass, a minificação do CSS e a concatenação em um único arquivo.

2. **Cópia do HTML:**
   - A tarefa `copiarHTML` simplesmente copia o arquivo HTML de origem (`src/index.html`) para o diretório de destino (`build`).

### Executando as Tarefas

Ao executar o comando `gulp` no terminal, ambas as tarefas são executadas em paralelo, otimizando o processo de construção do projeto.

Lembre-se de instalar as dependências do projeto com o comando:

```bash
npm install
```

Como Usar
Instalação das Dependências:

Execute npm install no terminal para instalar as dependências do projeto.
Execução das Tarefas do Gulp:

Execute gulp no terminal para iniciar as tarefas do Gulp.
Resultados:

Os arquivos otimizados serão gerados no diretório build.
O arquivo HTML estará diretamente em build, e o CSS estará em build/css.
Agora, seu projeto está pronto para ser utilizado, e as tarefas automatizadas garantem que o código CSS esteja otimizado e pronto para ser integrado no arquivo HTML principal.
