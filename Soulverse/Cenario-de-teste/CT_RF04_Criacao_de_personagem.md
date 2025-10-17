# Cenário 04: Criação de Personagem

## Caso de Teste 01: Criar personagem Shinigami com sucesso

| ID | Descrição |
|----|------------|
| C04-CT01 | O usuário deve conseguir criar um personagem da classe Shinigami com sucesso. |

### Pré-condições
- Usuário deve estar logado no sistema.  
- Usuário deve estar na tela de criação de personagem.

### Passos
1. **DADO** que estamos na tela de criação de personagem.  
2. **E** digitamos um nome válido no campo “Nome do personagem”.  
3. **E** selecionamos a classe **Shinigami**.  
4. **E** escolhemos uma **Zanpakutou**.  
5. **E** escolhemos aparência e sexo.  
6. **QUANDO** clicamos no botão **“Criar”**.  
7. **ENTÃO** o personagem deve ser criado com sucesso e adicionado à lista.

### Critérios de aceitação
- O personagem aparece na tela de seleção de personagens.  
- A classe, Zanpakutou e aparência correspondem ao que foi selecionado.  
- O redirecionamento para a tela de seleção ocorre corretamente.

---

## Caso de Teste 02: Criar personagem Hollow, Quincy ou Ryoka

| ID | Descrição |
|----|------------|
| C04-CT02 | O usuário deve conseguir criar um personagem de outra classe sem necessidade de selecionar Zanpakutou. |

### Pré-condições
- Usuário logado no sistema.  
- Tela de criação de personagem aberta.

### Passos
1. **DADO** que estamos na tela de criação de personagem.  
2. **E** digitamos um nome válido.  
3. **E** selecionamos uma classe diferente de Shinigami (Hollow, Quincy ou Ryoka).  
4. **E** escolhemos aparência e sexo.  
5. **QUANDO** clicamos em **“Criar”**.  
6. **ENTÃO** o personagem é criado com sucesso.

### Critérios de aceitação
- O campo de Zanpakutou não é obrigatório.  
- O personagem é exibido corretamente na seleção.

---

## Caso de Teste 03: Tentar criar personagem sem nome

| ID | Descrição |
|----|------------|
| C04-CT03 | O sistema deve impedir a criação de personagem sem nome. |

### Pré-condições
- Usuário logado no sistema.  
- Tela de criação de personagem aberta.

### Passos
1. **DADO** que estamos na tela de criação de personagem.  
2. **E** deixamos o campo “Nome do personagem” em branco.  
3. **E** selecionamos classe, aparência e sexo.  
4. **QUANDO** clicamos em **“Criar”**.  
5. **ENTÃO** uma mensagem de erro é exibida.

### Critérios de aceitação
- O personagem não é criado.  
- Deve aparecer a mensagem "Mínimo de 3 caracteres para nome do personagem".

---

## Caso de Teste 04: Tentar criar personagem com nome já existente

| ID | Descrição |
|----|------------|
| C04-CT04 | O sistema deve impedir a criação de personagem com o mesmo nome. |

### Pré-condições
- Usuário logado no sistema.

### Passos
1. **DADO** que estamos na tela de criação de personagem.
2. **E** digitamos um nome já existente.
2. **QUANDO** clicamos no botão **“Criar”**.  
3. **ENTÃO** uma mensagem de erro é exibida.

### Critérios de aceitação
- Nenhum personagem é criado.  
- Deve aparecer a mensagem "Sorry.But that name is in use!".

---

## Caso de Teste 05: Cancelar criação de personagem

| ID | Descrição |
|----|------------|
| C04-CT05 | O usuário deve poder cancelar a criação de personagem. |

### Pré-condições
- Usuário logado no sistema.

### Passos
1. **DADO** que estamos na tela de criação de personagem.  
2. **QUANDO** clicamos no botão **“X”** (fechar).  
3. **ENTÃO** a criação é cancelada e retornamos para a tela de seleção de personagem.

### Critérios de aceitação
- Nenhum personagem é criado.  
- Retorna corretamente para a tela anterior.


