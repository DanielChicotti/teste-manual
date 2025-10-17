# Cenário 03: Seleção de Personagem

## Caso de Teste 01: Selecionar personagem existente

| ID | Descrição |
|----|------------|
| C03-CT01 | O usuário deve conseguir selecionar um personagem existente e entrar no jogo. |

### Pré-condições
- Usuário deve estar logado no sistema.  
- Deve existir ao menos um personagem criado.

### Passos
1. **DADO** que estamos na tela de seleção de personagem.  
2. **E** existe ao menos um personagem criado.  
3. **QUANDO** clicamos sobre um personagem.  
4. **E** clicamos no botão **“Usar”**.  
5. **ENTÃO** o jogo deve carregar a conta/personagem selecionado e entrar no ambiente de jogo.

### Critérios de aceitação
- O personagem selecionado é carregado com sucesso.  
- Não há erros de carregamento ou travamentos.  
- O usuário é redirecionado corretamente para o ambiente de jogo.

---

## Caso de Teste 02: Tentar usar um slot vazio

| ID | Descrição |
|----|------------|
| C03-CT02 | O sistema deve trocar o botão "Usar" para "Criar" caso o usuário selecione um slot vazio. |

### Pré-condições
- Usuário deve estar logado no sistema.  
- Deve haver ao menos um slot vazio na tela.

### Passos
1. **DADO** que estamos na tela de seleção de personagem.  
2. **E** existe um slot vazio.  
3. **QUANDO** clicamos no slot vazio.  
4. **E** clicamos no botão **“Criar”**.  
5. **ENTÃO** deve ser redirecionado para a tela de criação de personagem.

### Critérios de aceitação
- A tela de criação de personagem deve ser carregada normalmente.  
- Nenhuma mensagem deve aparecer.  

---

## Caso de Teste 03: Deletar personagem existente

| ID | Descrição |
|----|------------|
| C03-CT03 | O usuário deve conseguir deletar um personagem existente. |

### Pré-condições
- Usuário deve estar logado no sistema.  
- Deve haver ao menos um personagem criado.

### Passos
1. **DADO** que estamos na tela de seleção de personagem.  
2. **E** existe um personagem criado.  
3. **QUANDO** clicamos sobre o personagem.  
4. **E** clicamos no botão **“Deletar”**.  
5. **E** confirmamos a ação.  
6. **ENTÃO** o personagem deve ser removido da lista.

### Critérios de aceitação
- O personagem desaparece da tela após a confirmação.  
- Uma mensagem de sucesso é exibida.  
- O slot pode ser reutilizado para criar um novo personagem.

---

## Caso de Teste 04: Cancelar deleção de personagem

| ID | Descrição |
|----|------------|
| C03-CT04 | O usuário deve poder cancelar a exclusão de um personagem. |

### Pré-condições
- Usuário deve estar logado no sistema.  
- Deve haver ao menos um personagem criado.

### Passos
1. **DADO** que estamos na tela de seleção de personagem.  
2. **E** existe um personagem criado.  
3. **QUANDO** clicamos sobre o personagem.  
4. **E** clicamos no botão **“Deletar”**.  
5. **E** clicamos em **“Cancelar”** na janela de confirmação.  
6. **ENTÃO** o personagem permanece na lista.

### Critérios de aceitação
- Nenhuma exclusão é realizada.  
- A lista de personagens não sofre alterações.  
- O personagem continua utilizável.

---

## Caso de Teste 05: Voltar para a tela de login

| ID | Descrição |
|----|------------|
| C03-CT05 | O usuário deve conseguir voltar à tela de login através do botão “Voltar”. |

### Pré-condições
- Usuário deve estar logado no sistema.

### Passos
1. **DADO** que estamos na tela de seleção de personagem.  
2. **QUANDO** clicamos no botão **“Voltar”**.  
3. **ENTÃO** o sistema deve retornar para a tela de login.

### Critérios de aceitação
- O redirecionamento ocorre corretamente.  
- Nenhum erro ou travamento ocorre no retorno.

---

## Caso de Teste 06: Scroll da lista de personagens

| ID | Descrição |
|----|------------|
| C03-CT06 | O usuário deve conseguir rolar a lista de personagens caso haja mais do que cabe na tela. |

### Pré-condições
- Usuário logado.  
- Lista de personagens com mais de 4 slots preenchidos.

### Passos
1. **DADO** que estamos na tela de seleção de personagem.  
2. **QUANDO** utilizamos a barra de rolagem lateral.  
3. **ENTÃO** os personagens ocultos devem aparecer na tela.

### Critérios de aceitação
- A rolagem é suave e responsiva.  
- Todos os personagens são exibidos corretamente.

---

## Caso de Teste 07: Clique fora dos botões

| ID | Descrição |
|----|------------|
| C03-CT07 | O sistema não deve executar nenhuma ação ao clicar em áreas vazias da interface. |

### Pré-condições
- Sistema online.

### Passos
1. **DADO** que estamos na tela de seleção de personagem.  
2. **QUANDO** clicamos fora dos campos de texto ou botões.  
3. **ENTÃO** nenhuma ação deve ser executada.

### Critérios de aceitação
- Nenhum evento inesperado ocorre.  
- Interface permanece inalterada.


