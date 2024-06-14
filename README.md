# RealTimeChatSystem

## Descrição

Este é um projeto criado para fins de estudo e por hobby. Desenvolvi o projeto com Laravel, Swoole, Octane, Livewire, Laravel Sail e Laravel Breeze, com o intuito de estudar e praticar essas tecnologias específicas. O desafio que eu propus consistiu em criar uma aplicação que permita aos usuários autenticados trocar mensagens instantâneas em tempo real.

<!-- ## Documentation -->

<!-- A documentação de API completa do projeto está disponível [aqui](https://exemplo.com/documentacao). -->

<!-- You can view the complete API documentation of the project after running it locally. Please run the project and access the Swagger documentation. [http://localhost/api/documentation](http://localhost/api/documentation). -->

## Funcionalidades

Aqui estão as principais funcionalidades do projeto:

1. **Registro de Usuários:** Os usuários podem criar uma conta no sistema fornecendo as informações necessárias.
2. **Login e Autenticação:** Os usuários podem fazer login no sistema usando suas credenciais.
3. **Logout** Os usuários podem sair do sistema, encerrando sua sessão atual.


<!-- ## Tecnologias Utilizadas

O projeto XYZ utiliza as seguintes tecnologias e práticas:

1. **Banco de Dados SQL:** O sistema utiliza um banco de dados SQL para armazenar informações dos usuários e outros dados relevantes.
2. **Cache Redis:** Para melhorar o desempenho, consultas frequentes são armazenadas em cache utilizando o Redis.
3. **Microserviços:** Algumas funcionalidades específicas são implementadas como microserviços independentes para garantir escalabilidade e modularidade.
4. **Framework MVC:** O projeto é construído usando um framework MVC (Model-View-Controller) para separar a lógica de negócios, a interface do usuário e a manipulação de dados.
5. **API RESTful:** A comunicação entre o frontend e o backend é realizada através de uma API RESTful, seguindo as melhores práticas de design de API.
6. **Testes Automatizados:** O projeto possui uma suíte de testes automatizados para garantir a estabilidade e a qualidade do código. -->

### Requisitos

Antes de executar o projeto em seu ambiente de desenvolvimento, certifique-se de ter os seguintes requisitos atendidos:

- **WSL:** O projeto requer que você esteja usando Linux ou o WSL (Windows Subsystem for Linux) se estiver usando Windows.
- **Docker ou Docker Engine:** É necessário ter o Docker ou o Docker Engine instalado em seu ambiente. O Docker é uma plataforma que permite empacotar e distribuir aplicações em contêineres.

### Instalação e Configuração Local

Para instalar e configurar o projeto localmente, siga as etapas abaixo:

1. Clone este repositório em sua máquina local.

2. Certifique-se de que o Docker está em execução no seu ambiente de desenvolvimento.

3. Execute o seguinte comando no terminal para instalar as dependências do projeto:
     ```bash
     docker run --rm \
         -u "$(id -u):$(id -g)" \
         -v "$(pwd):/var/www/html" \
         -w /var/www/html \
         laravelsail/php82-composer:latest \
         composer install --ignore-platform-reqs
     ```
     Para mais informações, consulte a [documentação do Laravel Sail](link_laravel_sail).

4. Crie o arquivo `.env` e configure suas variáveis de ambiente com o seguinte comando no terminal:
     ```bash
     cp .env.example .env
     ```  
5. Para iniciar o ambiente de desenvolvimento, execute o comando no terminal:
     ```bash
     ./vendor/bin/sail up
     ```  

6. Após iniciar o laravel sail, execute o comando para criar uma chave de criptografia e adicioná-la ao seu arquivo .env:
    ```    
    ./vendor/bin/sail artisan key:generate
    ```

7. No terminal, após criar seu banco de dados com base nas suas variaveis de ambiente configuradas, execute para realizar as migrações do banco de dados:
     ```bash
     ./vendor/bin/sail artisan migrate
     ```

8. Para encerrar o ambiente de desenvolvimento, execute no terminal:
     ```bash
     ./vendor/bin/sail down
     ```  

<!-- ## External Resources -->

<!-- During the development of the OpenPersonalFinanceAPI, the following external resources were used: -->

<!-- - [Biblioteca X](https://exemplo.com/biblioteca-x): Descrição da biblioteca X.
- [API de Pagamento Y](https://exemplo.com/api-pagamento-y): Integração com a API de pagamento Y para processar transações financeiras.
- [Framework Z](https://exemplo.com/framework-z): Utilização do framework Z para agilizar o desenvolvimento. -->
<!-- - [Swagger](https://swagger.io/): Swagger is used to document APIs. -->


<!-- ## Licença

O projeto XYZ é licenciado sob a Licença MIT. Consulte o arquivo [LICENSE](https://github.com/seu-usuario/projeto-xyz/blob/main/LICENSE) para obter mais informações.   -->

## Modelagem de Banco de dados

[Visualizar Modelagem](./public/tabelas.pdf)

