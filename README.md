# :scroll: SampleNodeLambda

Um simples microsserviço em Node entregue na AWS utilizando o serverless framework

---

## Inicializando
    Primeiramente é necessário uma conta na AWS devidamente configurada e o serverless framework instalado

    npm install serverless -g

    Se você ainda não tem uma conta AWS dê uma olhada aqui : 
  - [Como criar sua conta AWS](https://aws.amazon.com/pt/free/activate-your-free-tier-account/)

    É necessário que sua conta tenha as seguintes permissões:
        - AmazonDynamodbFullAccess
        - AWSCloudFormationFullAccess
        - AWSLambdaFullAccess
        - IAMFullAccess
        - AmazonAPIGatewayAdministrator

    Configure o framework para utilizar as credenciais da sua conta AWS
    serverless config credentials --provider aws --key <your_access_key> --secret <your_secret_key>

    Agora é hora de clonar o projeto e instalar as dependências necessárias

    git clone https://github.com/matheustex/SampleLambdaNode
    npm install

## Build

    serverless package

## Deploy

    serverless deploy

## Custom Deploy

    serverless deploy --stage stage --region region

## AWS Resources

  - [CloudFormation Stack](https://console.aws.amazon.com/cloudformation/home?region=us-east-1#/stacks/arn%3Aaws%3Acloudformation%3Aus-east-1%3A140981404942%3Astack%2FEventsSettings%2F091ab050-442a-11e9-81a5-126f3d94de7e/overview)
  - [CloudFront Distribution](https://console.aws.amazon.com/cloudfront/home?region=us-east-1#distribution-settings:E38817LJPYS8J6)
  - [Lambda Console](https://console.aws.amazon.com/lambda/home?region=us-east-1#functions/EventsSettings)