# Customização do osTicket com Docker

Este projeto contém as especificações básicas para executar uma instância padrão do osTicket em português do Brasil em um ambiente Docker. Além da construção inicial do Docker, há uma segunda etapa de configuração via interface gráfica que requer um servidor de banco de dados MySQL ou MariaDB disponível.

## Pré-requisitos

Certifique-se de ter os seguintes requisitos instalados antes de começar:

- [Docker](https://www.docker.com/)
- Servidor de Banco de Dados MySQL ou MariaDB

## Instalação

1. Clone este repositório:

   ```bash
   git clone https://seurepositorio.com/custom-osticket-docker.git
   ```

1. Navegue até o diretório do projeto:

    ```bash
    cd custom-osticket-docker
    ```

1. Construa a imagem do container

    ```bash
    docker compose -f docker-compose.dev.yml build
    ```

1. Inicie os containers:

    ```bash
    docker-compose up -d
    ```

1. Acesse a interface gráfica no navegador para a segunda etapa de configuração.

## Configuração Adicional

Após iniciar os containers, abra seu navegador e vá para: http://localhost:8080/setup

Siga as instruções na interface para configurar o osTicket e conectar ao seu servidor de banco de dados.

Nota: Certifique-se de colocar os dados de acesso e credenciais compatíveis com os utilizados no arquivo `docker-compose.dev.yml`.

Licença
Este projeto é licenciado sob a licença Affero General Public License (AGPLv3).