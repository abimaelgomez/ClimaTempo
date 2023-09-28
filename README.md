# NodeRed Weather API Consumer

Este é um guia passo a passo para configurar e usar uma API Node-RED que consome a "Weather API" para obter informações em tempo real sobre o clima de cidades em todo o mundo. A "Weather API" é uma API externa que fornece dados meteorológicos atualizados.


Requisitos

Antes de começar, certifique-se de que você tenha o seguinte instalado:
    
    - Node-RED - Uma plataforma de automação de código aberto baseada em Node.js.

    - Uma chave de API da "Weather API" (disponível em weatherapi.com).

    

Passo 1: Instalação e Configuração do Node-RED
    
    - Instale o Node-RED seguindo as instruções de instalação apropriadas para o seu sistema operacional.

    - Inicie o Node-RED executando o comando node-red no terminal.
![image](https://github.com/abimaelgomez/ClimaTempo/assets/123669805/6f384e34-bf21-4710-9362-b0b19e17db06)

    - Abra o ambiente Node-RED no seu navegador, geralmente em http://localhost:1880.
![image](https://github.com/abimaelgomez/ClimaTempo/assets/123669805/f978e4e6-c05c-4677-bf37-c4a64c5f0ec8)
![image](https://github.com/abimaelgomez/ClimaTempo/assets/123669805/dc759af5-01cc-40bb-a4b2-1f8f55b64e10)



Passo 2: Importação do Fluxo Node-RED

    - Para economizar tempo na configuração, você pode importar um fluxo Node-RED pré-configurado que já consome a "Weather API".

    - No ambiente Node-RED, clique no menu superior direito e selecione "Import".

    - Cole o conteúdo do arquivo JSON do fluxo pré-configurado que você pode encontrar em algum lugar dentro do seu projeto ou baixar da fonte onde você o encontrou.
    - O conteúdo do fluxo pré-configurado deve incluir todos os nós necessários para a comunicação com a "Weather API" e o tratamento dos dados.

    - Clique em "Import" para importar o fluxo.

    
Site API: https://openweathermap.org/api 
Passo 3: Configuração da Chave de API
    
    - Para que a API Node-RED possa se comunicar com a "Weather API", você precisa configurar a chave de API que você obteve da "Weather API".
    
    - Devemos no cadastrar para usar a APiKey de graça"

    - Localize o nó que faz a solicitação à "Weather API" no seu fluxo Node-RED.

    - Clique duas vezes no nó para abrir suas configurações.

    - Insira a chave de API na configuração apropriada.

    - Salve as alterações.

Passo 4: Configuração do Endpoint da Weather API
    
    - Verifique se o endpoint da "Weather API" está corretamente configurado no seu fluxo Node-RED. O endpoint é geralmente fornecido pela documentação da API.

    - Localize o nó que contém as configurações do endpoint da "Weather API".

    - Verifique se o URL do endpoint está correto.

    - Certifique-se de que quaisquer parâmetros de consulta (como cidade ou código postal) estejam configurados corretamente, de acordo com as suas necessidades.

    - Salve as alterações.

    

Passo 5: Execução e Teste
    
    - Agora que tudo está configurado, é hora de testar sua API Node-RED que consome a "Weather API".

    - Inicie o fluxo Node-RED clicando no botão "Deploy" no canto superior direito do ambiente Node-RED.

    - Crie uma rota de solicitação HTTP para sua API Node-RED, se ainda não existir. Isso permitirá que você faça solicitações para sua API e obtenha dados meteorológicos em tempo real.

    - Acesse sua API usando uma ferramenta como curl, Postman ou um navegador da web. Certifique-se de incluir os parâmetros necessários, como a cidade ou o código postal.

    -Escolhi a cidade de SP usando id da cidade destacado abaixo, então todos os dados consumidos serão da cidade de São Paulo em tempo real.
![image](https://github.com/abimaelgomez/ClimaTempo/assets/123669805/99677d4b-449a-4c0e-ab09-30f1e2f79d75)
        


    - Analise os resultados e verifique se você está recebendo os dados meteorológicos corretos da "Weather API".
![ObjetoJSOn](https://github.com/abimaelgomez/ClimaTempo/assets/123669805/334658a4-1bdd-4c60-bb2f-7bc387152466)


    - Após configurar o DashBoard ficará assim:
Podemos acessar o dashboard pelo end-point: 
http://127.0.0.1:1880/ui
![DashBoard](https://github.com/abimaelgomez/ClimaTempo/assets/123669805/c08ccef1-01d1-4276-b8dd-910ac42cc69d)

    
