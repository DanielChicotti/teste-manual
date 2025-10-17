# 📋 Requisitos Funcionais Detalhados para Testes Manuais

---

## 🔐 RF01 - Autenticação de Usuário

**Descrição:**  
O sistema deve permitir que o jogador acesse sua conta utilizando nome de usuário e senha válidos.

- O sistema deve permitir login com nome de usuário e senha corretos.  
- O sistema deve exibir mensagem de erro caso o login falhe.  
- O FPS deve ser exibido no canto superior da tela de login.  
- O botão “Entrar” só deve ficar ativo quando os campos obrigatórios estiverem preenchidos.

---

## 🆕 RF02 - Registro de Conta

**Descrição:**  
O sistema deve permitir que o usuário crie uma nova conta de acesso ao jogo.

- O sistema deve validar que nome de usuário e senha contenham no mínimo **3 caracteres**.  
- Caso os campos estejam em branco ou com menos de 3 caracteres, deve exibir mensagem de alerta.  
- O sistema deve impedir o cadastro de nomes de usuário duplicados.  
- Após o registro bem-sucedido, o usuário deve ser redirecionado para a tela de login.

**Funcionalidades esperadas:**  
- Campos: *Usuário*, *Senha* e *Repetir Senha*.  
- Mensagem de feedback em caso de erro ou sucesso.  
- Botão “Registrar” habilitado apenas com campos válidos.

---

## 🧙 RF03 - Seleção de Personagem

**Descrição:**  
Após o login bem-sucedido, o usuário deve acessar a tela de seleção de personagem.

- O sistema deve listar os personagens disponíveis da conta.  
- O botão “Entrar” deve estar disponível apenas ao selecionar um personagem válido.  
- Deve existir opção para retornar à tela de login.

**Funcionalidades esperadas:**  
- Exibição dos personagens criados.  
- Botão de seleção funcional.  
- Botão “Voltar” funcional.

---

## ✨ RF04 - Criação de Personagem

**Descrição:**  
O sistema deve permitir que o usuário crie um novo personagem em um slot vazio.

- O usuário deve informar nome, classe, gênero e aparência do personagem.  
- O sistema deve validar nome duplicado e campos obrigatórios.  
- Após a criação, o personagem deve aparecer automaticamente na tela de seleção.  
- O FPS deve permanecer visível.

**Funcionalidades esperadas:**  
- Campos para configuração do personagem.  
- Validação de nome.  
- Feedback visual em caso de sucesso ou falha.  
- Botão “Criar” habilitado apenas com campos válidos.

---

## 🧭 RF05 - Navegação Entre Telas

**Descrição:**  
O sistema deve permitir que o usuário navegue entre as telas de login, registro, seleção e criação de personagem de forma fluida.

- Botões de “Voltar” e “Registrar” devem redirecionar corretamente.  
- A navegação não deve apresentar travamentos.  
- As informações de FPS devem permanecer visíveis.

**Funcionalidades esperadas:**  
- Links e botões responsivos.  
- Feedback visual nas mudanças de tela.  
- Manutenção de performance.

---
