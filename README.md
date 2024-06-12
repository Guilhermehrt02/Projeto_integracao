O projeto desktop será constituído pelas seguintes telas e funcionalidades:
1. Tela Login (Exatamente igual a capacitação anterior)
2. Tela home: Terá um navbar (escolher posição) que irá ter botões home,
perfil, produtos e sair.
3. Em qualquer tela que tiver se apertar em home, voltará para essa tela inicial.
4. Tela perfil: Aqui serão mostradas as informações cadastradas pelo usuário no
momento de cadastro de conta.
5. Tela de produtos (Qualquer tipo de produto de escolha do grupo ou alguma
outra ideia mas que deve seguir os mesmos princípios): Nessa tela serão
mostrados todos os produtos da seguinte forma (podem seguir o Gama):
a. Visualização: Será feito em tabela com as seguintes colunas: Nome,
descrição, valor e edição.
b. Exclusão: Após apertar em editar terá a possibilidade de excluir.
c. Edição: Após apertar em editar abrirá uma nova tela contendo as
informações cadastradas e se for feito alguma edição dos dados nessa
tela, será habilitado o botão salvar.
d. Inserção: Botão que ficará na parte superior da tela com o intuito de
cadastrar algum produto (Seguir o exemplo do Gama e inserir uma
foto de identificação)
6. Botão sair: Retornará para a tela de login.
7. Instalação
Clone o repositório e navegue até o diretório do projeto:
git clone https://github.com/Guilhermehrt02/Projeto_integracao.git
Instale as dependências do projeto:
npm install
Configuração
Crie um arquivo src/environments/environment.ts e adicione as configurações do Firebase:

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
Executando o Projeto
Para iniciar a aplicação em modo de desenvolvimento, execute:
ng serve
A aplicação estará disponível em http://localhost:4200.

Estrutura do Projeto
src/app/components: Contém os componentes do projeto (Login, Home, Perfil, Produtos).
src/app/services: Contém os serviços utilizados para comunicação com o Firebase.
src/environments: Contém as configurações de ambiente (desenvolvimento e produção).
Componentes
Tela Login
Autenticação: Permite autenticar com Google ou email pessoal.
Rota: /login
Tela Home
Navbar: Contém botões para navegar entre Home, Perfil, Produtos e Sair.
Rota: /home
Tela Perfil
Informações do Usuário: Mostra as informações cadastradas no momento do registro.
Rota: /perfil
Tela de Produtos
Visualização: Tabela com Nome, Descrição, Valor e Edição.
Edição/Exclusão: Permite editar ou excluir produtos.
Inserção: Botão para adicionar novos produtos.
Rota: /produtos
Botão Sair
Função: Desloga o usuário e retorna à tela de login.

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

## Instalação

Clone o repositório e navegue até o diretório do projeto:
```bash
git clone https://github.com/Guilhermehrt02/Projeto_integracao.git
cd Projeto_integracao
