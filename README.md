# AWS-CloudFormation
 Este repositório faz parte do desafio proposto pela DIO, com o objetivo de consolidar os conhecimentos sobre AWS CloudFormation

# O que é o AWS CloudFormation

O AWS CloudFormation é um serviço que automatiza a criação, configuração e gerenciamento de recursos da AWS — tudo isso usando código.

Ou seja: em vez de clicar manualmente no console da AWS para criar recursos (como EC2, S3, VPCs, etc.), você descreve toda a infraestrutura em um arquivo de texto — chamado template — e o CloudFormation faz o resto por você.

Esse conceito é conhecido como Infraestrutura como Código (IaC – Infrastructure as Code).

# Como funciona

Você cria um template (em YAML ou JSON):

nele, você define os recursos que quer criar (por exemplo: um bucket S3, uma instância EC2 e um grupo de segurança).

Você envia esse template para o CloudFormation:

ele lê o arquivo, entende as configurações e cria uma Stack (um conjunto organizado de recursos interdependentes).

O CloudFormation provisiona tudo automaticamente:

ele cuida da ordem de criação, dependências, permissões e rollback se algo der errado.

# Vantagens de usar o CloudFormation

Automação completa da infraestrutura
Padronização entre ambientes (dev, test, prod)
Facilidade de replicação — o mesmo template pode ser usado várias vezes
Controle de versões com Git (IaC versionada)
Rollback automático em caso de erro
Integração com DevOps (CodePipeline, CodeDeploy, etc.)

# Ciclo de uso do CloudFormation

Crie o template →

Faça upload no CloudFormation →

Execute a stack →

CloudFormation cria todos os recursos →

(Opcional) Atualize ou delete a stack
