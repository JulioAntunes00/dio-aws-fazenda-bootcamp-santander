# RELATÓRIO DE IMPLEMENTAÇÃO DE SERVIÇOS AWS

Data: 13/01/2026
Empresa: Abstergo Industries
Responsável: Julio Antunes Santos de Oliveira

## Introdução
Este relatório apresenta o processo de implementação de ferramentas na empresa Abstergo Industries, realizado por Julio Antunes Santos de Oliveira. O objetivo do projeto foi elencar 3 serviços AWS, com a finalidade de realizar a diminuição de custos imediatos. A estratégia foca na **troca de despesas de capital (CapEx)** — como a compra de servidores físicos — por **despesas variáveis (OpEx)**, pagando apenas pelo que for utilizado na nuvem.

## Descrição do Projeto
O projeto de implementação de ferramentas foi dividido em 3 etapas, cada uma com seus objetivos específicos. A seguir, serão descritas as etapas do projeto:

Etapa 1: 
- Nome da ferramenta: Amazon EC2 (Elastic Compute Cloud)
- Foco da ferramenta: Computação na Nuvem e Servidores Virtuais.
- Descrição de caso de uso: O EC2 será utilizado para hospedar a aplicação de gestão da fazenda. Diferente do modelo tradicional ("on-premise"), onde precisaríamos comprar um servidor superdimensionado, usaremos instâncias EC2 com **Modelo Sob Demanda**. Isso permite que a fazenda desligue os servidores fora do horário comercial ou durante a entressafra, gerando economia real e eliminando a necessidade de "adivinhar a capacidade" necessária da infraestrutura.

Etapa 2:
- Nome da ferramenta: Amazon S3 (Simple Storage Service)
- Foco da ferramenta: Armazenamento de Objetos Altamente Escalável.
- Descrição de caso de uso: Utilizaremos o S3 para armazenar backups, imagens de drones e documentos fiscais. A implementação focará na criação de "Buckets" seguros. A grande vantagem estratégica é a **Durabilidade e Disponibilidade** dos dados, garantindo que informações críticas da safra não sejam perdidas por falhas de hardware local, além de oferecer custo de armazenamento muito inferior ao de manter Storage Area Networks (SAN) físicas.

Etapa 3:
- Nome da ferramenta: Amazon RDS (Relational Database Service)
- Foco da ferramenta: Banco de Dados Gerenciado.
- Descrição de caso de uso: O RDS será implementado para gerenciar os dados estruturados de estoque e financeiro. Ao optar por este serviço gerenciado, aplicamos o **Modelo de Responsabilidade Compartilhada**: a AWS cuida do "trabalho pesado" (instalação, patches de segurança e backups do banco), permitindo que nossa equipe de TI foque apenas na otimização da aplicação e suporte aos usuários, sem perder tempo com manutenção de S.O. de banco de dados.

## Conclusão
A implementação de ferramentas na empresa Abstergo Industries tem como esperado a modernização da infraestrutura, permitindo maior agilidade e elasticidade para acompanhar o crescimento da produção agrícola. A substituição do data center local pela AWS reduz a carga operacional da equipe de TI e transforma custos fixos elevados em custos variáveis previsíveis. Recomenda-se a continuidade dos estudos sobre **AWS Security Groups** para garantir a segurança da rede nesta nova topologia.



Assinatura do Responsável pelo Projeto:

Julio Antunes Santos de Oliveira