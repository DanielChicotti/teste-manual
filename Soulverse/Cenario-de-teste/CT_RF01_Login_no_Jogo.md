# Cenário 01: Login no jogo SoulVerse

## Caso de Teste 01: Login com credenciais válidas

| ID        | Descrição                                                        |
|-----------|------------------------------------------------------------------|
| C01-CT01  | O login será realizado com um nome de usuário e senha válidos.    |

### Pré-condições
- O servidor do jogo deve estar **Online**.
- O usuário deve possuir uma conta registrada.

### Passos
1. **DADO** que estamos na tela de login do jogo.
2. E preenchemos o campo **Usuário** com `Conta01`.
3. E preenchemos o campo **Senha** com `senha123`.
4. **QUANDO** clicamos no botão **“Entrar”**.
5. **ENTÃO** devemos ser redirecionados para a seleção de persongem.

### Critérios de aceitação
- O redirecionamento para a seleção de personagem deve ocorrer corretamente.
- Nenhuma mensagem de erro deve aparecer.
- A lista de personagem deve ser exibido no centro da tela.

---

## Caso de Teste 02: Tentativa de login com senha incorreta

| ID        | Descrição                                                        |
|-----------|------------------------------------------------------------------|
| C01-CT02  | O login deve falhar quando a senha estiver incorreta.            |

### Pré-condições
- O servidor deve estar **Online**.
- O usuário deve possuir conta registrada.

### Passos
1. **DADO** que estamos na tela de login.
2. E preenchemos o campo **Usuário** com `jogadorTeste`.
3. E preenchemos o campo **Senha** com `senhaErrada`.
4. **QUANDO** clicamos em **“Entrar”**.
5. **ENTÃO** deve ser exibida uma mensagem de erro.

### Critérios de aceitação
- A mensagem “You've entered an incorrect password” deve aparecer.
- O login não deve ser efetuado.

---

## Caso de Teste 03: Tentativa de login com servidor offline

| ID        | Descrição                                                        |
|-----------|------------------------------------------------------------------|
| C01-CT03  | O login deve falhar quando o servidor estiver offline.           |

### Pré-condições
- O servidor deve estar **Offline**.

### Passos
1. **DADO** que estamos na tela de login.
2.  E preenchemos os campos corretamente.
3. **QUANDO** clicamos em **“Entrar”**.
4. **ENTÃO** deve aparecer um alerta de falha de conexão.

### Critérios de aceitação
- Mensagem: “Servidor indisponível. Tente novamente mais tarde.”
- O login não deve ser efetuado.

---

## Caso de Teste 04: Campos de login vazios

| ID        | Descrição                                                        |
|-----------|------------------------------------------------------------------|
| C01-CT04  | O sistema deve validar se os campos estão preenchidos.          |

### Pré-condições
- O servidor deve estar **Online**.

### Passos
1. **DADO** que estamos na tela de login.
2. E deixamos os campos de Usuário e/ou Senha vazios.
3. **QUANDO** clicamos em **“Entrar”**.
4. **ENTÃO** deve ser exibida uma mensagem de validação.

### Critérios de aceitação
- Mensagem exibida: “Mínimo de 3 letras para usuário ou senha”.
- O login não deve ser efetuado.
