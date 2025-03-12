# Rota Escolar - Resumo de Funcionamento do Software

**Observação:** Este documento descreve as funcionalidades garantidas 100% no sistema. Outras funcionalidades estão planejadas para futuras implementações, dependendo de tempo e outros fatores.

## Objetivo

O **Rota Escolar** foi desenvolvido para atender às necessidades de transportadores escolares, oferecendo uma solução completa que otimiza a gestão e operação do transporte escolar.

## Tecnologias Utilizadas

- **Flutter & Dart:**  
  Utilizados para o desenvolvimento da interface e funcionalidades, possibilitando a criação de uma solução multiplataforma.

- **Firebase:**  
  - **Hospedagem:** A versão web é hospedada na nuvem, assegurando alta disponibilidade e escalabilidade.  
  - **Banco de Dados:** Responsável pelo armazenamento e gerenciamento seguro dos dados em nuvem.  
  - **Autenticação de Usuários:** Gerencia o acesso e garante a segurança dos usuários nas plataformas web e Android.

- **Cloud Run:**  
  Utilizado como webhook de comunicação entre o Stripe e o Firebase Realtime Database, garantindo a atualização automática de informações de pagamentos e assinaturas.

- **APIs:**  
  - **Brevo:** Utilizada para envio de e-mails automáticos, como notificações de reajuste de mensalidade.  
  - **Stripe:** Implementada para gerenciamento de pagamentos e assinaturas recorrentes.
 
![Imagem do WhatsApp de 2025-03-11 à(s) 15 57 21_2119be74](https://github.com/user-attachments/assets/b96fc91f-93f4-45ca-a76e-1fa01b1e20c2)

## Plataformas

- **Web:**  
  Acesso via navegador com integração completa das funcionalidades suportadas pelo Firebase.
  
- **Android:**  
  Versão mobile que integra autenticação e demais funcionalidades, mantendo a consistência com a versão web.

## Detalhamento das Funcionalidades por Página

### Tela de Login

- **Login no App:**  
  Permite que o usuário insira suas credenciais (usuário e senha) para acessar o aplicativo.

![screencapture-9000-idx-rota-escolar-1740271762534-cluster-uf6urqn4lned4spwk4xorq6bpo-cloudworkstations-dev-2025-03-11-15_33_43](https://github.com/user-attachments/assets/4a8933b2-af67-4eec-aaf9-970d4c1007f1)
  
- **Recuperação de Senha:**  
  Disponibiliza uma funcionalidade para que o usuário recupere sua senha em caso de esquecimento, facilitando o restabelecimento do acesso ao app.

![screencapture-9000-idx-rota-escolar-1740271762534-cluster-uf6urqn4lned4spwk4xorq6bpo-cloudworkstations-dev-2025-03-11-15_34_24](https://github.com/user-attachments/assets/f34d3f9d-f0f0-46fc-a5b2-1adfc4f21143)

### Tela de Registro

- **Registro de Usuário:**  
  Permite que novos usuários criem uma conta no aplicativo, inserindo informações como nome, e-mail, senha e demais dados necessários para o cadastro.

![screencapture-9000-idx-rota-escolar-1740271762534-cluster-uf6urqn4lned4spwk4xorq6bpo-cloudworkstations-dev-2025-03-11-15_34_01](https://github.com/user-attachments/assets/c7e99d0d-e7c5-4e77-b900-117bf5d771b8)

### Dashboard

- **Resumo de Informações Importantes:**  
  Exibição de dados organizados em gráficos para fornecer uma visão geral da operação do transporte escolar, com métricas essenciais para auxiliar o transportador na tomada de decisões.

![screencapture-9000-idx-rota-escolar-1740271762534-cluster-uf6urqn4lned4spwk4xorq6bpo-cloudworkstations-dev-2025-03-11-15_38_33](https://github.com/user-attachments/assets/51fd307f-881b-4872-8875-da9659c83412)
![screencapture-9000-idx-rota-escolar-1740271762534-cluster-uf6urqn4lned4spwk4xorq6bpo-cloudworkstations-dev-2025-03-11-15_38_50](https://github.com/user-attachments/assets/1574791d-35af-4201-b63b-58e2b451f1cd)


### Escolas

- **Registro de Escolas:**  
  Permite o cadastro de novas escolas no sistema.
  
- **Edição de Escolas:**  
  Possibilita a alteração dos dados das escolas cadastradas.
  
- **Exclusão de Escolas:**  
  Permite a remoção de escolas do sistema quando necessário.
  
- **Pesquisa de Escolas por Nome:**  
  Facilita a busca por escolas cadastradas utilizando o nome como critério.
  
- **Envio de Mensagens para Escola via WhatsApp:**  
  Permite a comunicação direta com a escola através do WhatsApp.

![screencapture-9000-idx-rota-escolar-1740271762534-cluster-uf6urqn4lned4spwk4xorq6bpo-cloudworkstations-dev-2025-03-11-15_35_10](https://github.com/user-attachments/assets/2acd3e1c-e779-4d8c-8068-fa514e2ad5a4)

### Alunos

- **Registro de Alunos:**  
  Permite o cadastro de novos alunos no sistema.
  
- **Edição de Alunos:**  
  Possibilita a alteração dos dados dos alunos cadastrados.
  
- **Exclusão de Alunos:**  
  Permite a remoção de alunos do sistema quando necessário.
  
- **Pesquisa de Aluno por Nome:**  
  Facilita a busca por alunos cadastrados utilizando o nome como critério.
  
- **Envio de Mensagem para o Responsável via WhatsApp:**  
  Permite a comunicação direta com o responsável do aluno através do WhatsApp.

![screencapture-9000-idx-rota-escolar-1740271762534-cluster-uf6urqn4lned4spwk4xorq6bpo-cloudworkstations-dev-2025-03-11-15_35_31](https://github.com/user-attachments/assets/baea1005-41c9-47c7-a4a1-07bdad4c8342)

### Reajuste

- **Aplicação de Reajuste de Mensalidade:**  
  Permite aplicar reajuste nos valores das mensalidades para alunos selecionados.
  
- **Envio de E-mail de Aviso:**  
  Integração com a API Brevo para envio automático de notificações sobre reajustes aos responsáveis.
  
- **Pesquisa de Alunos:**  
  Permite buscar alunos por nome ou valor da mensalidade.

![screencapture-9000-idx-rota-escolar-1740271762534-cluster-uf6urqn4lned4spwk4xorq6bpo-cloudworkstations-dev-2025-03-11-15_35_43](https://github.com/user-attachments/assets/6e5b99ee-a617-4615-907f-6ac794144fe4)

### Convite

- **Definição de Valor do Convite:**  
  Permite que o transportador defina o valor do convite para novos alunos.
  
- **Envio de Convite para Cadastro:**  
  Envio de um link para que o responsável do aluno se auto cadastre via página web.


### Gastos

- **Cadastro de Gastos:**  
  Permite registrar despesas relacionadas à operação do transporte escolar.
  
- **Edição e Exclusão de Gastos:**  
  Possibilita a modificação ou remoção de registros de gastos.
  
- **Filtragem por Categoria e Período:**  
  Organização e análise dos gastos mensalmente, categorizando as despesas.

![screencapture-9000-idx-rota-escolar-1740271762534-cluster-uf6urqn4lned4spwk4xorq6bpo-cloudworkstations-dev-2025-03-11-15_36_00](https://github.com/user-attachments/assets/d04c8657-cc16-44f0-ad17-4d15ca02dac0)

### Avisos de Pagamento

- **Listagem de Pagamentos:**  
  Lista os pagamentos das mensalidades dos alunos, concluídos ou não.
  
- **Cobranças:**  
  Permite a realização de cobranças via WhatsApp dos responsáveis que tiveram atraso nas mensalidades.

![screencapture-9000-idx-rota-escolar-1740271762534-cluster-uf6urqn4lned4spwk4xorq6bpo-cloudworkstations-dev-2025-03-11-15_36_21](https://github.com/user-attachments/assets/b2ddd471-e80e-4818-b153-34424056ab5a)

### Assinatura

- **Realização de Assinatura:**  
  Funcionalidade para assinar planos que liberam recursos extras no aplicativo.
  
- **Integração com API Stripe:**  
  Permite pagamentos seguros e recorrentes via Stripe.

![screencapture-9000-idx-rota-escolar-1740271762534-cluster-uf6urqn4lned4spwk4xorq6bpo-cloudworkstations-dev-2025-03-11-15_36_35](https://github.com/user-attachments/assets/880965e5-bf74-4e6b-953e-30afdefbe5c6)

### Perfil

- **Informações do Usuário:**  
  Exibição e edição dos dados do usuário cadastrado no sistema.
  
- **Logout:**  
  Permite que o usuário encerre sua sessão com segurança, garantindo a proteção dos dados e acessos.
  
- **Exclusão de Conta:**  
  Funcionalidade que permite ao usuário excluir sua conta do sistema, removendo todos os seus dados de forma permanente.

![screencapture-9000-idx-rota-escolar-1740271762534-cluster-uf6urqn4lned4spwk4xorq6bpo-cloudworkstations-dev-2025-03-11-15_36_59](https://github.com/user-attachments/assets/159067cd-fdac-441c-96d0-f5352063abf4)

