# Requisitos do Sistema

## 1. Introdução
Este documento descreve os requisitos funcionais e não funcionais para o desenvolvimento da plataforma de entregas Ilha Delivery. O objetivo do sistema é substituir a comunicação via WhatsApp pelo acompanhamento estruturado de pedidos, similar ao iFood, permitindo o rastreamento e gerenciamento de entregas.

## 2. Requisitos Funcionais
### **1. Cadastro e Autenticação**

- **RF01** - O sistema deve permitir o cadastro de usuários (clientes e entregadores).
- **RF02** - O sistema deve permitir login e autenticação dos usuários.
- **RF03** - O administrador deve poder cadastrar entregadores e definir permissões.

### **2. Gerenciamento de Pedidos**

- **RF04** - O cliente deve poder criar um pedido informando endereço de entrega, descrição e foto dos produtos.
- **RF05** - O sistema deve permitir que o pedido seja atribuído a um entregador automaticamente ou manualmente.
- **RF06** - O cliente deve poder acompanhar o status do pedido em tempo real.
- **RF07** - O entregador deve poder atualizar o status do pedido (ex.: "Em trânsito", "Entregue").
- **RF08** - O sistema deve permitir que o cliente avalie a entrega e o entregador.

### **3. Notificações e Comunicação**

- **RF09** - O sistema deve enviar notificações push para os usuários sobre o status do pedido.
- **RF10** - O entregador deve receber notificações quando um novo pedido for atribuído a ele.
- **RF11** - O sistema deve permitir que clientes e entregadores se comuniquem via chat.

### **4. Painel Administrativo**

- **RF12** - O administrador deve poder visualizar todos os pedidos e seu status.
- **RF13** - O sistema deve permitir exportação de relatórios de entregas.
- **RF14** - O administrador deve poder gerenciar os entregadores e clientes.

### **5. Integração com APIs Externas**

- **RF15** - O sistema deve integrar-se à API do iFood para importar pedidos automaticamente.
- **RF16** - O sistema deve permitir integração com serviços de pagamento online (Pix, cartão de crédito).

## 3. Requisitos Não Funcionais
### **1. Desempenho e Escalabilidade**

- **RNF01** - O sistema deve suportar pelo menos 1000 usuários simultâneos.
- **RNF02** - O tempo de resposta para qualquer operação não deve exceder 3 segundos.

### **2. Segurança**

- **RNF03** - O sistema deve utilizar autenticação JWT para login seguro.
- **RNF04** - Os dados sensíveis devem ser armazenados de forma criptografada.
- **RNF05** - O sistema deve ter um mecanismo de recuperação de senha via e-mail.

### **3. Usabilidade e Acessibilidade**

- **RNF06** - O aplicativo deve seguir boas práticas de UI/UX para facilitar a navegação dos usuários.
- **RNF07** - O sistema deve ser responsivo, adaptando-se a diferentes tamanhos de tela.

### **4. Manutenibilidade e Tecnologia**

- **RNF08** - O backend deve ser desenvolvido em Django + Django Rest Framework.
- **RNF09** - O frontend do aplicativo deve ser desenvolvido em React Native.
- **RNF10** - O código deve ser modular para facilitar futuras atualizações.
