# Trabalho para conclusão do curso

Cloud Computing AWS

*Escola da Nuvem*

https://novaislary.github.io/siteCurriculos/

# Site Estático AWS

Este repositório contém um site estático hospedado na Amazon Web Services (AWS), utilizando serviços como Amazon S3, CloudFront, Shield e Route 53. Este README fornecerá uma visão geral do projeto, instruções para configuração e implementação, bem como informações adicionais sobre os serviços AWS utilizados.

## Visão Geral

O site estático é uma aplicação web simples que consiste em arquivos HTML, CSS, JavaScript e outros recursos estáticos. Ele é projetado para fornecer informações estáticas aos visitantes, sem a necessidade de um backend dinâmico.

Os principais serviços AWS utilizados neste projeto são:

- **Amazon S3**: Armazenamento de objetos usado para hospedar e servir os arquivos estáticos do site.
- **Amazon CloudFront**: Rede de entrega de conteúdo (CDN) para distribuir o conteúdo do site de forma rápida e eficiente.
- **AWS Shield**: Serviço de proteção contra ataques DDoS (Distributed Denial of Service) para garantir a segurança do site.
- **Amazon Route 53**: Serviço de DNS para configurar e gerenciar o domínio do site.

## Configuração e Implantação

Siga as etapas abaixo para configurar e implantar o site estático na AWS:

1. **Crie um bucket no Amazon S3**: Acesse o console da AWS, vá para o serviço S3 e crie um novo bucket. Nomeie o bucket de acordo com o nome de domínio que deseja usar para o site.

2. **Faça upload dos arquivos estáticos**: Após criar o bucket, faça upload dos arquivos estáticos do site para o bucket. Certifique-se de que os arquivos estejam configurados como públicos para que possam ser acessados por meio da web.

3. **Configurar o site estático**: No console do S3, vá para as configurações do bucket e ative o site estático. Defina o documento de índice como o arquivo HTML principal do site.

4. **Habilitar o CloudFront**: Acesse o console da AWS, vá para o serviço CloudFront e crie uma nova distribuição. Configure a origem como o bucket S3 criado anteriormente e defina as configurações adicionais, como cache, segurança e domínios personalizados.

5. **Configurar o DNS com o Route 53**: Vá para o console do Route 53 e crie uma nova zona hospedada. Em seguida, crie um novo registro de alias para o domínio desejado e associe-o à distribuição do CloudFront criada anteriormente.

6. **Ativar o AWS Shield**: O AWS Shield é um serviço integrado e não requer configurações adicionais. No entanto, é importante estar ciente de que ele fornece proteção contra ataques DDoS.

Após seguir essas etapas, o site estático estará configurado e implantado na AWS. Verifique se o domínio está acessível e funcional após a propagação completa do DNS.

## Recursos Adicionais

- Documentação do Amazon S3: [https://docs.aws.amazon.com/AmazonS3](https://docs.aws.amazon.com/AmazonS3)
- Documentação do Amazon CloudFront: [https://docs.aws.amazon.com/CloudFront](https://docs.aws.amazon.com/CloudFront)
- Documentação do AWS Shield:
