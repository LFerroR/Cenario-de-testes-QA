## Cenário 07: Registro de ponto (Controle de Horas) pelo módulo Time.

### Caso de Teste 01: Marcar ponto (Check In) com horário válido.

| ID       | Descrição                                                                  |
| :------- | :------------------------------------------------------------------------- |
| C07-CT01 | O sistema deve permitir que o usuário registre sua entrada com sucesso.    |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| O usuário deve estar logado e ter acesso ao módulo "Time".    |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o usuário acessa o menu \"Time > Attendance > Punch In\" |
| **E** verifica que o horário atual é válido                     |
| **QUANDO** clicar em \"Punch In\"                               |
| **ENTÃO** o registro de entrada deve ser salvo com sucesso      |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| O sistema deve confirmar o registro com uma mensagem e salvar o horário. |

---

### Caso de Teste 02: Tentar marcar ponto sem horário permitido ou fora do expediente.

| ID       | Descrição                                                                 |
| :------- | :------------------------------------------------------------------------ |
| C07-CT02 | O sistema deve impedir o registro de entrada fora do horário permitido.   |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| O usuário deve estar fora do horário permitido para entrada.  |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o usuário acessa o menu \"Punch In\" fora do horário permitido |
| **QUANDO** tentar registrar o ponto                             |
| **ENTÃO** o sistema deve exibir uma mensagem de erro ou restrição |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| O sistema deve impedir o registro e apresentar mensagem adequada. |

---

### Caso de Teste 03: Consultar registro de ponto anterior.

| ID       | Descrição                                                              |
| :------- | :---------------------------------------------------------------------- |
| C07-CT03 | O sistema deve permitir que o usuário consulte registros de ponto anteriores. |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| O usuário deve ter ao menos um registro de ponto anterior.    |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o usuário acessa o menu \"Time > Attendance > My Records\" |
| **QUANDO** selecionar uma data anterior                         |
| **ENTÃO** o sistema deve exibir os registros de entrada e saída da data selecionada |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| O sistema deve exibir corretamente os registros existentes da data informada. |

## 🔗 Evidências (Jam.dev)

- **C01-CT01** → [Execução](https://jam.dev/c/5ca66892-ca00-477d-bc2f-75d450873baf)  
- **C01-CT02** → [Execução](https://jam.dev/c/458bfd4c-b33d-4f59-885b-28b76686dc80)  
- **C01-CT03** → [Execução](https://jam.dev/c/23e27e64-0131-4171-8548-19c6dc48bc4e) 
