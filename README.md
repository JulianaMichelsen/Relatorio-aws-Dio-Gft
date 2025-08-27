# RELATÓRIO DE IMPLEMENTAÇÃO DE SERVIÇOS AWS

**Data:** 27 de Agosto de 2025  
**Empresa:** Abstergo Industries  
**Responsável:** Juliana Michelsen  

## Introdução
Este relatório apresenta o processo de implementação de ferramentas na empresa Abstergo Industries, realizado por Juliana Michelsen. O objetivo do projeto foi *elencar 3 serviços AWS*, com a finalidade de tecnologias utilizadas no bootcamp da DIO/GFT como Java e AWS, será implementada microserviços visando uma solução escalável, de baixo custo e com gerenciamento de filas de mensagens.

## Descrição do Projeto
O projeto de implementação de ferramentas foi dividido em 3 **etapas**, cada etapa com seus objetivos específicos. A seguir, serão descritas as etapas do projeto:

### Etapa 1:
- **AWS Lambda**  
- **Foco da ferramenta:** Criação de funções de código sem a necessidade de provisionar ou gerenciar servidores.  
- **Descrição de caso de uso:** Uma função Lambda em Java será o coração da API. Ela irá processar as requisições HTTP recebidas, gerenciar a lógica de negócios e interagir com o banco de dados e a fila de mensagens. Isso garante uma arquitetura escalável, onde a função é executada apenas quando necessário, otimizando os custos e também outra vantagem é deixar a funcionalidades desacopladas facilitando a manutenção e a criação de novas features.

### Etapa 2:
- **Amazon DynamoDB**  
- **Foco da ferramenta:** Um banco de dados NoSQL de chave-valor e documentos totalmente gerenciado, projetado para alto desempenho em qualquer escala.  
- **Descrição de caso de uso:** O DynamoDB será utilizado para armazenar os dados da aplicação. Sua capacidade de lidar com grandes volumes de dados e sua natureza sem servidor o tornam a escolha ideal para uma API de alta performance, complementando a arquitetura baseada em Lambda.

### Etapa 3:
- **AWS SQS**  
- **Foco da ferramenta:** Um serviço de enfileiramento de mensagens totalmente gerenciado, que permite desacoplar e dimensionar microserviços, sistemas distribuídos e aplicativos sem servidor.  
- **Descrição de caso de uso:** O SQS será utilizado para gerenciar a fila de mensagens entre os componentes da aplicação. Isso é crucial para processos assíncronos, garantindo que as requisições sejam processadas de forma confiável, mesmo durante picos de tráfego, e que a aplicação continue responsiva.

## Conclusão
A implementação dessa arquitetura Serverless com AWS Lambda, Amazon DynamoDB e Amazon SQS resultará em uma solução altamente escalável e eficiente para a Abstergo Industries. Espera-se que essa abordagem reduza custos operacionais, aumente a resiliência do sistema e proporcione maior flexibilidade para futuros desenvolvimentos.

É recomendado o monitoramento contínuo da performance da API e a exploração de outros serviços AWS para otimizar ainda mais a solução.

