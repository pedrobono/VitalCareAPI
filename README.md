# VitalCareAPI
Descrição do Projeto

Nome do Projeto: Sistema de Gestão de Atendimentos Médicos

Tecnologias Utilizadas:

    Spring Boot para desenvolvimento do backend

    RESTful API para comunicação entre os sistemas

    GraphQL para consultas eficientes de dados

    MongoDB como banco de dados NoSQL

    Docker para containerização do projeto

Objetivo do Projeto: Este projeto visa implementar uma aplicação backend simples, utilizando as tecnologias Spring Boot, MongoDB, Docker, RESTful e GraphQL, para demonstrar conceitos de construção de sistemas de saúde. O sistema será utilizado para gerenciar o cadastro de usuários, pacientes e atendimentos médicos, com funcionalidades específicas para diferentes papéis de usuários.

Funcionalidades:

    Cadastro de Usuários:

        Os usuários podem ser cadastrados com os papéis de médico, enfermeiro ou gerente.

        A autenticação e a autorização serão baseadas no papel de cada usuário, garantindo que as permissões de acesso sejam restritas conforme o papel.

    Cadastro de Pacientes:

        O sistema permitirá o cadastro de pacientes, com informações básicas de identificação e histórico.

    Cadastro de Atendimentos Médicos:

        O médico e a enfermeira poderão registrar sinais vitais e queixas dos pacientes.

        Somente o médico poderá adicionar diagnósticos ao atendimento e encerrá-lo.

        Após o diagnóstico ser realizado, o médico pode encerrar o atendimento, mas a enfermeira será responsável por finalizar o processo de encerramento do atendimento.

    Histórico de Pacientes:

        Todos os atendimentos realizados ficam registrados para o histórico do paciente, permitindo que o médico ou o gerente possam consultar os atendimentos anteriores.

    Uso de MongoDB:

        O MongoDB será utilizado para o armazenamento dos dados de usuários, pacientes, atendimentos e históricos de maneira flexível e escalável.

    GraphQL:

        A API irá expor endpoints RESTful para operações CRUD básicas, mas também contará com uma interface GraphQL para consultas complexas, como a busca por atendimentos ou histórico de um paciente.

    Dockerização:

        O projeto será containerizado usando Docker para garantir que o ambiente de desenvolvimento e produção sejam consistentes e fáceis de configurar.

Objetivos de Aprendizado:

    Aprender e praticar a criação de uma API RESTful com Spring Boot.

    Integrar GraphQL ao backend para consultas de dados mais flexíveis e eficientes.

    Explorar o MongoDB como banco de dados NoSQL, adequado para armazenar documentos de forma escalável.

    Implementar a segurança e controle de acesso para diferentes papéis de usuários (médico, enfermeiro e gerente).

    Contenerizar a aplicação utilizando Docker, garantindo um ambiente de desenvolvimento padronizado e portabilidade.

Estrutura do Projeto:

    Camada de Controladores (Controller): Para expor os endpoints RESTful e GraphQL.

    Camada de Serviços (Service): Lógica de negócios para a manipulação de dados.

    Camada de Repositórios (Repository): Interface para interação com o banco de dados MongoDB.

    Camada de Segurança: Autenticação e autorização com base no papel de usuário.

    Docker: Arquivo Dockerfile e docker-compose.yml para configuração do ambiente de containers.

Conclusão: Este projeto tem como objetivo ser uma base para a construção de sistemas mais complexos de gestão de atendimentos médicos, utilizando práticas modernas de desenvolvimento de software, como APIs RESTful e GraphQL, além de containers Docker para facilitar a distribuição e implantação.