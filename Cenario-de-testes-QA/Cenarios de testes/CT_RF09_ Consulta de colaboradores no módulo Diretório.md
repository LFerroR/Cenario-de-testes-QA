## Cenário 09: Consulta de colaboradores no módulo Diretório.

### Caso de Teste 01: Buscar colaborador por nome com sucesso.

| ID       | Descrição                                                               |
| :------- | :---------------------------------------------------------------------- |
| C09-CT01 | O sistema deve retornar corretamente o colaborador pesquisado pelo nome. |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| O usuário deve estar logado no sistema.                       |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o usuário acessa o menu \"Directory\"              |
| **E** insere o nome de um colaborador existente no campo de busca |
| **QUANDO** clicar em \"Search\"                                 |
| **ENTÃO** o sistema deve exibir o colaborador correspondente à busca |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| O nome, cargo e localização do colaborador devem ser exibidos corretamente. |

---

### Caso de Teste 02: Buscar colaborador inexistente.

| ID       | Descrição                                                                   |
| :------- | :-------------------------------------------------------------------------- |
| C09-CT02 | O sistema deve exibir uma mensagem apropriada quando nenhum colaborador for encontrado. |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| O usuário deve estar logado no sistema.                       |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o usuário acessa o menu \"Directory\"              |
| **E** digita um nome que não corresponde a nenhum colaborador    |
| **QUANDO** clicar em \"Search\"                                 |
| **ENTÃO** uma mensagem como \"No Records Found\" deve ser exibida |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| O sistema deve exibir claramente que não há registros encontrados. |

---

### Caso de Teste 03: Aplicar filtro por cargo (Job Title).

| ID       | Descrição                                                                |
| :------- | :------------------------------------------------------------------------ |
| C09-CT03 | O sistema deve permitir a filtragem de colaboradores por cargo.           |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| O usuário deve estar logado e o sistema deve conter dados de funcionários. |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o usuário acessa o menu \"Directory\"              |
| **E** seleciona um cargo no campo \"Job Title\"                 |
| **QUANDO** clicar em \"Search\"                                 |
| **ENTÃO** apenas os colaboradores com o cargo selecionado devem ser listados |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| O filtro deve funcionar corretamente e retornar apenas resultados válidos. |

## 🔗 Evidências (Jam.dev)

- **C01-CT01** → [Execução](https://jam.dev/c/b4c0b0ac-c40e-4e12-9fc8-1036cc4d6e11)  
- **C01-CT02** → [Execução](https://jam.dev/c/529ca406-5e4e-4b97-82d3-0bc220907ba9)  
- **C01-CT03** → [Execução](https://jam.dev/c/03a0baf8-df4d-4344-a480-2ee0ddbd2761) 
