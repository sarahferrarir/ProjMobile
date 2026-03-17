# Histórias de usuário

> Baseado no protótipo no [figma](https://www.figma.com/design/MimwF67MobMdDzxx0bPGPg/Condominio-Cidade-Jardins?node-id=0-1&t=6yR8PW6jcOwSiXYK-1)
## Funcionalidade: Agendamento de Quadras
**Como** um morador do condomínio Cidade Jardins   
**Eu quero** reservar quadras esportivas   
**Para** organizar meu horário de uso das áreas comuns  

---
###  Cenário 1: Realizar Login

- **Dado que** estou na tela inicial  
- **E** possuo um usuário e senha cadastrados  
- **Quando** eu insiro minhas credenciais  
- **Então** devo acessar a tela principal do aplicativo  

---

### Cenário 2: Visualizar Quadras Disponíveis

- **Dado que** estou na tela inicial do app  
- **Quando** acesso a opção “Reservar Quadra”  
- **Então** devo visualizar as quadras disponíveis:  
  - Tênis (5 disponíveis)  
  - Poliesportivas (3 disponíveis)  
  - Futebol (2 disponíveis)  

---

### Cenário 3: Selecionar Tipo de Quadra

- **Dado que** estou na tela de seleção de quadras  
- **Quando** escolho o tipo de quadra desejada  
- **Então** devo ser direcionado para a tela de agendamento  

---

### Cenário 4: Escolher Data e Horário

- **Dado que** estou na tela de agendamento  
- **E** visualizo os horários disponíveis  
- **Quando** seleciono uma data e um horário livre  
- **Então** devo poder prosseguir com a reserva  

---

### Cenário 5: Confirmar Reserva

- **Dado que** selecionei uma quadra, data e horário
- **E** estou com o condomínio em dia  
- **Quando** clico em “Confirmar”  
- **Então** a reserva deve ser registrada no sistema  
- **E** devo visualizar uma mensagem de confirmação  

### Cenário 5.1: Bloqueio de Reserva por Inadimplência

- **Dado que** selecionei uma quadra, data e horário  
- **E** não estou com o condomínio em dia  
- **Quando** clico em “Confirmar”  
- **Então** a reserva não deve ser realizada  
- **E** devo visualizar uma mensagem informando a pendência de pagamento

---

### Cenário 6: Visualizar Minhas Reservas

- **Dado que** já realizei reservas
- **E** estou na tela principal do app
- **Quando** acesso a opção “Minhas Reservas”  
- **Então** devo visualizar todas as minhas reservas ativas  

---

### Cenário 7: Cancelar Reserva

- **Dado que** estou na tela “Minhas Reservas”  
- **Quando** seleciono a opção “Cancelar” em uma reserva  
- **Então** a reserva deve ser removida  
- **E** o horário deve voltar a ficar disponível

---
### Cenário 8: Deslogar 
- **Dado que** estou na tela principal do app
- **Quando** seleciono o ícone "sair" 
- **Então** devo ser deslogado do app
- **E** devo ser redirecionado para a tela inicial de login  
