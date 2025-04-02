# Requisitos do Sistema

## 1. Introdução
Este documento descreve os requisitos funcionais e não funcionais para o desenvolvimento da plataforma de entregas Ilha Delivery. O objetivo do sistema é substituir a comunicação via WhatsApp pelo acompanhamento estruturado de pedidos, similar ao iFood, permitindo o rastreamento e gerenciamento de entregas.

## 2. Requisitos Funcionais
### 2.1. Cadastro e Autenticação
- [ ] O sistema deve permitir o cadastro de clientes.
- [ ] O sistema deve permitir o cadastro de estabelecimentos (restaurantes, lojas e e-commerces).
- [ ] O sistema deve permitir que entregadores se cadastrem.
- [ ] O sistema deve permitir login e autenticação segura para clientes, estabelecimentos e entregadores.
- [ ] O sistema deve suportar login via e-mail/senha e autenticação via redes sociais ou OTP (One-Time Password).

### 2.2. Gestão de Pedidos
- [ ] O cliente deve poder visualizar os estabelecimentos disponíveis.
- [ ] O cliente deve poder selecionar produtos e adicionar ao carrinho.
- [ ] O cliente deve poder personalizar pedidos (exemplo: adicionar/remover ingredientes).
- [ ] O sistema deve permitir que o cliente finalize a compra e realize o pagamento pelo app.
- [ ] O sistema deve notificar o estabelecimento sobre novos pedidos.
- [ ] O estabelecimento deve poder aceitar, preparar e atualizar o status do pedido.
- [ ] O entregador deve receber notificações sobre pedidos disponíveis para entrega.
- [ ] O cliente deve receber notificações sobre mudanças no status do pedido.

### 2.3. Rastreamento e Comunicação
- [ ] O cliente deve poder visualizar o status da entrega em tempo real.
- [ ] O sistema deve atualizar automaticamente os status do pedido, como:
  - Chegou ao galpão do Ilha Delivery
  - Em trânsito para a ilha
  - Chegou na ilha
  - Em rota para entrega
  - Entregue
- [ ] O cliente e o entregador devem poder se comunicar diretamente dentro do app.
- [ ] O sistema deve permitir que o cliente avalie a entrega e o estabelecimento após a finalização do pedido.

### 2.4. Histórico e Relatórios
- [ ] O cliente deve poder visualizar o histórico de pedidos.
- [ ] O sistema deve gerar relatórios para os estabelecimentos sobre pedidos e vendas.
- [ ] O sistema deve permitir que os administradores gerenciem usuários e estabelecimentos.

## 3. Requisitos Não Funcionais
### 3.1. Segurança
- [ ] O sistema deve implementar criptografia para armazenamento de senhas.
- [ ] O sistema deve garantir transações seguras utilizando protocolos como HTTPS e TLS.
- [ ] O sistema deve seguir boas práticas de proteção contra ataques como SQL Injection e XSS.

### 3.2. Desempenho
- [ ] O sistema deve ser escalável para suportar um grande número de usuários simultâneos.
- [ ] O tempo de resposta para ações críticas (login, atualização de status de pedidos) deve ser inferior a 2 segundos.

### 3.3. Usabilidade
- [ ] A interface deve ser intuitiva e de fácil navegação para diferentes perfis de usuários.
- [ ] O sistema deve ser responsivo, funcionando corretamente em dispositivos móveis e desktops.

### 3.4. Integrações
- [ ] O sistema deve permitir integração com gateways de pagamento.
- [ ] O sistema deve permitir integração com serviços de rastreamento de entrega.
- [ ] O sistema deve permitir integração com marketplaces como Amazon para atualização de status de pedidos.

## 4. Perguntas e Considerações
1. O sistema permitirá pedidos programados ou apenas pedidos em tempo real?
2. Haverá suporte para múltiplos meios de pagamento, como Pix, cartão de crédito e boleto?
3. Os estabelecimentos terão um painel administrativo para gerenciar seus pedidos?
4. Os clientes poderão cancelar pedidos após a confirmação?
5. Os entregadores terão um sistema de rating baseado nas entregas realizadas?
6. Haverá algum sistema de fidelidade ou cashback para incentivar o uso contínuo da plataforma?
