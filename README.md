# Plataforma de Gestão de Produtos McDonald's

Este projeto é uma aplicação de desktop desenvolvida em Angular que utiliza o Firebase para autenticação e operações CRUD (Criar, Ler, Atualizar, Deletar) em produtos do McDonald's. Este README fornecerá instruções básicas para configurar e executar o projeto.

## Funcionalidades

1. **Tela Login**: Possibilidade de autenticar com o Google ou com o email pessoal.
2. **Tela Home**: Contém uma navbar que inclui botões para Home, Perfil, Produtos e Sair.
3. **Tela Perfil**: Mostra as informações cadastradas pelo usuário no momento do cadastro de conta.
4. **Tela de Produtos**:
    - **Visualização**: Exibe os produtos em uma tabela com as seguintes colunas: Nome, Descrição, Valor e Edição.
    - **Exclusão**: Após apertar em editar, terá a possibilidade de excluir.
    - **Edição**: Após apertar em editar, abrirá uma nova tela contendo as informações cadastradas e, se for feita alguma edição dos dados nessa tela, será habilitado o botão salvar.
    - **Inserção**: Botão que ficará na parte superior da tela com o intuito de cadastrar algum produto (incluir uma foto de identificação).
5. **Botão Sair**: Retornará para a tela de login.

##Configuração

Crie um arquivo `src/environments/environment.ts` e adicione as configurações do Firebase:
```bash
export const environment = {
  production: false,
  firebase: {
    apiKey: "SUA_API_KEY",
    authDomain: "SEU_AUTH_DOMAIN",
    projectId: "SEU_PROJECT_ID",
    storageBucket: "SEU_STORAGE_BUCKET",
    messagingSenderId: "SEU_MESSAGING_SENDER_ID",
    appId: "SEU_APP_ID"
  }
};
```
##Estrutura do Projeto

1. **src/app/components:** Contém os componentes do projeto (Login, Home, Perfil, Produtos).
2. **src/app/services:** Contém os serviços utilizados para comunicação com o Firebase.
3. **src/environments:** Contém as configurações de ambiente (desenvolvimento e produção).



