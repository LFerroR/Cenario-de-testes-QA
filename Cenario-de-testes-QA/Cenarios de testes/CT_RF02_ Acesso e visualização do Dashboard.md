## Cenário 02: Acesso e visualização do Dashboard.

### Caso de Teste 01: Acesso ao Dashboard após login bem-sucedido.

| ID       | Descrição                                                        |
| :------- | :---------------------------------------------------------------- |
| C02-CT01 | Verificar a exibição correta do Dashboard após login com sucesso. |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| O usuário deve estar autenticado com credenciais válidas.     |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o usuário acessou o sistema com sucesso              |
| **QUANDO** for redirecionado automaticamente após o login         |
| **ENTÃO** a tela do Dashboard deve ser exibida com os atalhos e widgets principais |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| O sistema deve exibir corretamente a interface do Dashboard.     |

---

### Caso de Teste 02: Verificação da exibição dos widgets do Dashboard.

| ID       | Descrição                                                 |
| :------- | :-------------------------------------------------------- |
| C02-CT02 | Os widgets padrão devem ser exibidos corretamente no Dashboard. |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| O usuário deve estar na tela do Dashboard após login.         |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o usuário está autenticado                          |
| **E** está visualizando o Dashboard                              |
| **QUANDO** a página for carregada                                |
| **ENTÃO** widgets como \"Time at Work\" e \"My Actions\" devem ser exibidos |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| Todos os widgets principais devem ser visíveis e funcionais.     |

---

### Caso de Teste 03: Acesso ao Dashboard com sessão expirada.

| ID       | Descrição                                                            |
| :------- | :------------------------------------------------------------------- |
| C02-CT03 | O sistema deve redirecionar o usuário para o login se a sessão estiver expirada. |

| **Pré-condições**                                             |
| :------------------------------------------------------------ |
| O usuário estava logado, mas a sessão expirou.                |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que o usuário acessou o sistema anteriormente            |
| **E** permaneceu inativo por um longo período                    |
| **QUANDO** tentar acessar o Dashboard novamente                  |
| **ENTÃO** o sistema deve redirecioná-lo para a página de login    |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| A sessão expirada deve ser tratada corretamente com redirecionamento. |

## 🔗 Evidências (Jam.dev)

- **C01-CT01** → [Execução](https://jam.dev/c/8a3ad4a5-3ccc-4434-8b0d-802362d75634)  
- **C01-CT02** → [Execução](https://jam.dev/c/fff3c3d5-df0d-45ee-b71e-aca8a6fd12e3)  
- **C01-CT03** → [Execução](https://jam.dev/c/eb950592-f41c-4e69-8b66-8467264b8de9) 
