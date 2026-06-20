# Serviço de Processamento de Imagem na AWS (Gerador de Ícones)

Projeto acadêmico de um sistema em nuvem que recebe o upload de uma imagem, processa-a em uma instância EC2 e devolve um ícone pronto. O processamento remove o fundo da imagem original e aplica uma borda circular ao redor, transformando-a em um ícone.

## Visão geral

O sistema implementa um microsserviço de processamento de imagem hospedado em uma instância EC2. O usuário envia uma imagem comum, o serviço a manipula e o resultado final (o ícone) é armazenado para consulta posterior.

## Fluxo resumido:


1. O usuário faz o upload de uma imagem.
2. A instância EC2 recebe a imagem através de uma API REST.
3. O serviço remove o fundo da imagem.
4. O serviço adiciona uma borda circular, gerando o ícone.
5. O ícone final é salvo no armazenamento, e sua referência é registrada no banco de dados.