## Cenário 05: Gerenciamento de candidatos no módulo de Recrutamento.

### Caso de Teste 01: Adicionar um novo candidato com dados válidos.

| ID       | Descrição                                                              |
| :------- | :---------------------------------------------------------------------- |
| C05-CT01 | O sistema deve permitir adicionar um novo candidato com informações válidas. |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| O usuário deve estar logado e ter acesso ao módulo "Recruitment". |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o usuário acessa o menu \"Recruitment\"             |
| **E** clica em \"Add\"                                           |
| **E** preenche os campos obrigatórios (nome, vaga, e-mail)       |
| **QUANDO** clicar em \"Save\"                                    |
| **ENTÃO** o candidato deve ser adicionado à lista de candidatos  |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| O candidato deve ser exibido corretamente na lista após o cadastro. |

---

### Caso de Teste 02: Tentar adicionar candidato sem preencher campos obrigatórios.

| ID       | Descrição                                                                     |
| :------- | :------------------------------------------------------------------------------ |
| C05-CT02 | O sistema deve exibir mensagens de erro ao tentar cadastrar um candidato sem preencher os campos obrigatórios. |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| O usuário deve estar logado no sistema.                       |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o usuário acessa o menu \"Recruitment\"             |
| **E** clica em \"Add\"                                           |
| **E** não preenche os campos obrigatórios                       |
| **QUANDO** clicar em \"Save\"                                    |
| **ENTÃO** mensagens de erro devem ser exibidas em cada campo obrigatório |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| Os campos obrigatórios devem ser validados com mensagens de erro. |

---

### Caso de Teste 03: Buscar candidato cadastrado pelo nome.

| ID       | Descrição                                                        |
| :------- | :---------------------------------------------------------------- |
| C05-CT03 | O sistema deve retornar corretamente um candidato pesquisado pelo nome. |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| O candidato deve estar cadastrado no sistema.                 |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o usuário acessa o menu \"Recruitment\"             |
| **E** digita o nome do candidato no campo de busca              |
| **QUANDO** clicar no botão \"Search\"                           |
| **ENTÃO** o sistema deve listar corretamente o candidato correspondente |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| O candidato pesquisado deve ser exibido na lista de resultados. |

## 🔗 Evidências (Jam.dev)

- **C01-CT01** → [Execução](https://jam.dev/c/2d3626d3-cc4b-4df6-94e5-5c8b2a835f07)  
- **C01-CT02** → [Execução](https://jam.dev/c/85559481-87cb-4659-9c23-071d31570643)  
- **C01-CT03** → [Execução](https://jam.dev/c/34dfc43b-bf53-4fe7-b91b-a9af58426e66) 
