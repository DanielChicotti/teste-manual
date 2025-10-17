# Cenário 01: Registro de Conta

## Caso de Teste 01: Criar conta com sucesso

| ID | Descrição |
|----|------------|
| C01-CT01 | O usuário deve conseguir criar uma conta informando dados válidos. |

### Pré-condições
- Sistema online.
- Não existir conta com o nome informado.

### Passos
1. **DADO** que estamos na tela de registro de conta.  
2. **QUANDO** preenchemos o campo **Usuário** com um nome válido.  
3. **E** preenchemos o campo **Senha** com pelo menos 3 caracteres.  
4. **E** repetimos a senha corretamente.  
5. **E** clicamos no botão **“Registrar”**.  
6. **ENTÃO** a conta é criada com sucesso e somos redirecionados para a tela de login.

### Critérios de aceitação
- Mensagem de sucesso exibida.  
- Login possível com as credenciais recém-criadas.  
- Nenhum erro ou travamento ocorre.

---

## Caso de Teste 02: Criar conta com nome de usuário já existente

| ID | Descrição |
|----|------------|
| C01-CT02 | O sistema deve impedir a criação de conta com nome de usuário já cadastrado. |

### Pré-condições
- Já existir uma conta com o nome informado.

### Passos
1. **DADO** que estamos na tela de registro de conta.  
2. **QUANDO** digitamos um nome de usuário já existente.  
3. **E** clicamos no botão **“Registrar”**.  
4. **ENTÃO** uma mensagem de erro é exibida informando que o nome já está em uso.

### Critérios de aceitação
- A conta não é criada.  
- A mensagem de erro é clara.  
- O usuário pode tentar novamente com outro nome.

---

## Caso de Teste 03: Criar conta com menos de 3 caracteres

| ID | Descrição |
|----|------------|
| C01-CT03 | O sistema deve impedir a criação de conta com nome ou senha menor que 3 caracteres. |

### Pré-condições
- Sistema online.

### Passos
1. **DADO** que estamos na tela de registro.  
2. **QUANDO** digitamos um nome ou senha com menos de 3 caracteres.  
3. **E** clicamos no botão **“Registrar”**.  
4. **ENTÃO** uma mensagem de erro é exibida informando a regra mínima.

### Critérios de aceitação
- Nenhuma conta é criada.  
- A regra de 3 caracteres é respeitada.  
- A mensagem é clara e visível.

---

## Caso de Teste 04: Senhas não coincidem

| ID | Descrição |
|----|------------|
| C01-CT04 | O sistema deve impedir a criação de conta quando as senhas não coincidem. |

### Pré-condições
- Sistema online.

### Passos
1. **DADO** que estamos na tela de registro.  
2. **QUANDO** digitamos uma senha no segundo campo diferente da primeira.  
3. **E** clicamos em **“Registrar”**.  
4. **ENTÃO** uma mensagem de erro é exibida informando que as senhas não coincidem.

### Critérios de aceitação
- Conta não é criada.  
- Mensagem clara é exibida.  
- Usuário pode corrigir os campos.

---

## Caso de Teste 05: Tentar registrar com campos em branco

| ID | Descrição |
|----|------------|
| C01-CT05 | O sistema deve impedir o registro quando houver campos obrigatórios em branco. |

### Pré-condições
- Sistema online.

### Passos
1. **DADO** que estamos na tela de registro.  
2. **QUANDO** deixamos um ou mais campos vazios.  
3. **E** clicamos em **“Registrar”**.  
4. **ENTÃO** uma mensagem de erro é exibida informando que todos os campos devem ser preenchidos.

### Critérios de aceitação
- Conta não é criada.  
- Mensagem clara e visível.  
- Botão “Registrar” permanece ativo para nova tentativa.

---

## Caso de Teste 06: Cancelar criação de conta

| ID | Descrição |
|----|------------|
| C01-CT06 | O usuário deve conseguir cancelar a criação da conta ao clicar no “X”. |

### Pré-condições
- Sistema online.

### Passos
1. **DADO** que estamos na tela de registro.  
2. **QUANDO** clicamos no botão **“X”** no canto superior direito.  
3. **ENTÃO** retornamos à tela de login.

### Critérios de aceitação
- Nenhuma conta é criada.  
- Retorno sem erros ou travamentos.

---

## Caso de Teste 07: Exibir regra mínima corretamente

| ID | Descrição |
|----|------------|
| C01-CT07 | A regra de “mínimo de 3 letras” deve ser exibida corretamente na tela de registro. |

### Pré-condições
- Sistema online.

### Passos
1. **DADO** que estamos na tela de registro.  
2. **QUANDO** observamos as informações abaixo dos campos de entrada.  
3. **ENTÃO** a mensagem **“Mínimo de 3 letras para Usuário e Senha”** deve estar visível e legível.

### Critérios de aceitação
- Texto exibido corretamente.  
- Mensagem posicionada de forma clara e não cortada.

---

## Caso de Teste 08: Clique fora dos botões

| ID | Descrição |
|----|------------|
| C01-CT08 | O sistema não deve executar nenhuma ação ao clicar em áreas vazias da interface. |

### Pré-condições
- Sistema online.

### Passos
1. **DADO** que estamos na tela de registro.  
2. **QUANDO** clicamos fora dos campos de texto ou botões.  
3. **ENTÃO** nenhuma ação deve ser executada.

### Critérios de aceitação
- Nenhum evento inesperado ocorre.  
- Interface permanece inalterada.
