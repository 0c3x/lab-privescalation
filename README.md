# Mini Laboratório para Treinar a Técnica de Escalada de Privilégio no Linux

Este repositório contém um mini laboratório que tem como objetivo auxiliar no aprendizado e treinamento da técnica de escalada de privilégio em sistemas Linux. O laboratório fornece um ambiente controlado para explorar alguns cenários e praticar habilidades de segurança.

## Iniciando o Laboratório

É importantante que tenha o Docker instalado em sua máquina, caso não tenha segue um tutorial: https://docs.docker.com/engine/install/ubuntu/

Siga as etapas abaixo para iniciar o laboratório:

1. Faça o clone do repositório com o seguinte comando:

git clone https://github.com/0c3x/lab-privescalation.git

2. Acesse com o terminal a pasta com o arquivo docker-compose.yml e inicie o ambiente executando o seguinte comando:

```
docker-compose up -d
```

Esse comando iniciará os containers necessários para o laboratório.

3. Acesse o ambiente interativo do laboratório:

```
docker-compose exec edu bash
```

Isso abrirá um shell interativo dentro do container do laboratório, permitindo que você execute comandos e realize as atividades práticas.

## Autor

Este repositório é mantido por [0c3x](https://www.linkedin.com/in/luan-carneiro-52128328a/). Se você tiver alguma dúvida, sugestão ou feedback, sinta-se à vontade para entrar em contato. Estou sempre aberto a contribuições e melhorias.

Happy hacking!
