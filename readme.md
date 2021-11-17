# O Projeto

A necessidade deste projeto é criar uma página de perguntas onde cada pergunta pode haver várias respostas.

# Necessidade

Você lembra daquela página chamada 'Ask'? 

> Esta rede social, permite que você envie perguntas para crush e o mais importante, de forma *anônima*, se você quiser e é claro!

![](/public/img/uau.gif)

Este projeto é uma página similar ao Ask. 

# Passo a passo:

#### Realize o download em algum locatório em seu computador. Após, abra a pasta em uma IDE de preferência, utilizei o VSCode e abra o terminal e digite o comando abaixo e aperte enter: 

```javascript
npm install
```

Para instalar todas as dependências. 

#### Próximo passo é, abrir uma IDE de Banco de Dados com mysql2, por exemplo, a MySQL Workbench que utilizei para este projeto. 

#### Verifique sua conexão com o usuário 'root', e, o hostname e porta.

#### Em seguida, vá na pasta *database* e abra o arquivo *database.js* e ajuste o host e a porta para o mesmo que usa em sua máquina.

#### A seguir, utilize o comando abaixo: 

```javascript
npm run dev
```

A tabela de *Perguntas* deverá ficar da seguinte forma: 

| id | titulo           | descricao                                         |
|----|------------------|---------------------------------------------------|
| 1  | Ask é bom?       |  Eis a questão.                                   |
| 2  | Sobre o pet café | Será que ele também é bonzinho quando estou fora? |

Já a tabela de *Respostas*, ficará assim: 

| id | corpo                                          | perguntaId |
|----|------------------------------------------------|------------|
| 1  | com certeza, é ótimo! ainda mais se crush usa. |      1     |
| 2  | eu não sei.                                    |      2     |
| 3  | eu espero que simm.                            |      2     |
| 4  | só sei que ele é muito doido.                  |      2     |

> 🛑 As tabelas são salvas na schema *guiaperguntas*, analise o arquivo *database.js*.

#### O servidor inciará na porta:8080 - acesse <http://localhost:8080>

Após isto, acesse o seu localhost e arrase! 

![](/public/img/piscada-rihanna.gif)
