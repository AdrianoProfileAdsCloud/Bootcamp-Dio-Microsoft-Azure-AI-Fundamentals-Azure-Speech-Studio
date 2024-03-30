# Dio - Microsoft Azure AI Fundamentals - Azure-Speech-Studio
Se trata de um projetinho de forma mais a nivel de apresentar o que foi aprendido no módulo Azure-Speech-Studio.Exploramos o uso do Azure Speech Studio e a análise linguística proporcionada pelo Language Studio.
"Aprofundei" o entendimento sobre como aproveitar essas ferramentas avançadas da Microsoft Azure. Tendo como foco aprimorar as habilidades na implementação de soluções de análise de fala e linguagem, o que proporcionou uma compreensão mais ampla e prática das capacidades oferecidas por essas tecnologias inovadoras.
A seguir vou realizando um passo a passo de como fiz essas implementações na prático no portal do Microsoft Azure.
Tendo como objetivo apenas mostrar meu entendimento. Tendo em vista que para tais passos que irei descrever abaixo e possível obter no site oficial da Microsoft.Aqui descrevo do meu modo, com base nos conhecimentos adquiridos nas aulas.

 ### Conversão de Audio em Texto.
 
Primeiro é preciso criar o Serviços Cognitivos.
Em seguida navegue para a página do Estúdio de fala em:
   https://speech.microsoft.com/, claro acessando com a mesa conta.

 Estando no Estudio de Fala seleciomos o idioma desejado.Em seguida escolhemos os arquivo(s) de audio a ser convertido(Conversão de fala em Texto.mp3). 
 
![Conversão de fala em Texto](https://github.com/AdrianoProfileAdsCloud/Azure-Speech-Studio/assets/141897391/58c8340e-a3cd-4624-9891-e0cd5780dd7a)

   Enão logo, será mostrado ao lado em Resultado de Teste a converão do audio para texto conforme o aúdio é executado.
   
![Exibição da Conversão de Fala em texto](https://github.com/AdrianoProfileAdsCloud/Azure-Speech-Studio/assets/141897391/cdb9451f-c0e1-48df-8cd9-08a3c2bad37b)

   Com este serviço é possivél converter qualquer audio em fala.Não só isso podemos fazer essa conversão do audio em qualquer idioma.
    No https://github.com/Azure-Samples/cognitive-services-speech-sdk ainda podemos ver com o sdk as implementações possíveis do serviço para algumas linguagens de programação e sistemas operacionais.

  ![Usando o Sdk do serviços de fala](https://github.com/AdrianoProfileAdsCloud/Azure-Speech-Studio/assets/141897391/9bed38b6-ef25-4bd2-acf6-07e4a4372096)
  
   Entre outras informações contidas ainda na mesma pagina do Estudio de fala - Conversação de fala em texo em tempo real.

   ![Proximas Etapas](https://github.com/AdrianoProfileAdsCloud/Azure-Speech-Studio/assets/141897391/c8720952-8b40-4ccc-b8a9-efd1a1c2c14c)


### Análise de Sentimentos com Language Studio no Azure AI.
   
  Consiste em analise Semantica de texto ou fala;precisamente análise de sentimentos.Dando-se pelo processamento da Linguagem Narural(PNL).
  É o ramo da IA que nos ajuda na interpretação de mensages, textos e liguagens de uma forma geral.

   Para tal, já logado no portal seguiremos alguns passos:
    1- Criar um Recurso. 
    2- Selecionar - AI + Machine Learning.
    3- Selecionar - Language service.
    
 ![Analise de Sentimentos ](https://github.com/AdrianoProfileAdsCloud/Azure-Speech-Studio/assets/141897391/660607b6-4bcc-4cd6-a4ea-19aeba67ee28)

    Na tela a seguir mostrará as Defauts features.
    Seguimos clicando em: Continue to create your resource.
    
 ![criar idioma](https://github.com/AdrianoProfileAdsCloud/Azure-Speech-Studio/assets/141897391/160eeaab-9f37-4d59-8540-8c0d08e34fc1)
 
   Observação: Uma coisa muito importante que deverá ser lembrada a todo instente é o Uso Responsável da IA.
![UsoResponsavelIA](https://github.com/AdrianoProfileAdsCloud/Azure-Speech-Studio/assets/141897391/2bac5e6d-ddd5-4d26-813a-300853226fad)

  Em seguida ao marcar o termo de uso Uso Responsável da IA. E só clicar e Revisar/criar
   A implantação do serviço começará.
   
   ![Processo de Implantação](https://github.com/AdrianoProfileAdsCloud/Azure-Speech-Studio/assets/141897391/e315bf9a-baf2-4d7f-aaaf-3a010bb2c54a)
   
   Após o termino da implantação navegar para o Language Cognitive em:
    https://language.cognitive.azure.com/home

   Obs: Em Resource name - Selecionar o resorce criado na etapa anterior.Para ser feito o link com o serviço a ser usado.
   
![languageCognitive](https://github.com/AdrianoProfileAdsCloud/Azure-Speech-Studio/assets/141897391/cdc71b7c-928e-46a0-b55d-047c781117c3)

   Como queremos analisar através do texto selecionado o grau de safistação por exemplo de um cliente em resposta a um serviço oferecido. Devemos então selecionar - Classify text - Analyze sentiment mine options.
   
![Classify Text](https://github.com/AdrianoProfileAdsCloud/Azure-Speech-Studio/assets/141897391/13b66f17-309e-4872-8c38-6caf3f457b43)

  Na próxima tela podemos trabalhar de duas formas:
   Entranos com o texto diretamente da área - Enter your own text, upload a file...
   Ou realizamos o upload do arquivo de texto que se deseja realizar a análise em - Arraste e solte arquivo(s)...
   
![language Studio](https://github.com/AdrianoProfileAdsCloud/Azure-Speech-Studio/assets/141897391/3f26670e-39af-4c55-89d0-25f48a51d27b)

   ### Ao analisar o texto contido no arquivo de texto Analise-Restaurante.txt(na pasta inputs), é possivél de imediato ter a resposta se os serviços prestados em geral agradou de forma positiva ou negativa o cliente.

   ![Analise - Restaurante](https://github.com/AdrianoProfileAdsCloud/Azure-Speech-Studio/assets/141897391/078fdc41-9550-42c7-ad1b-906780e982e3)

    Neste caso vemos após a analise que de forma geral o cliente ficou satifeito pois 78% correspponde que tudo ocorreu bem.
    Com uma parcela de 7% apenas dos serviços prestados estavam com algum problema.
    Tendo como Sentimento da frase(texto analisado, de acordo com o cliente) dado como positivo com confiaça de 94%.
     Manifestando a opinião sobre os pratos servidos com avaliações tido como deliciosos sinalando positividade.

   ### Ao analisar o texto contido no arquivo de texto Analise-Hotel.txt (na pasta inputs), é possivél de imediato ter a resposta se os serviços prestados em geral agradou de forma positiva ou negativa o cliente.

   ![Analise - Hotel](https://github.com/AdrianoProfileAdsCloud/Azure-Speech-Studio/assets/141897391/df192ac3-ebae-46b3-8d1d-7489113f2c66)

    Neste caso vemos após a analise que de forma geral o cliente ficou satifeito pois 96% correspponde que tudo ocorreu rasoavelmente bem nos na tratativa dos clientes.
    Com uma parcela de 3% corresponder como analise neutra.
    Tendo como Sentimento da frase(texto analisado, de acordo com o cliente) dado como positivo com confiaça de 96%.
     Manifestando a opinião sobre o Hotel Paríso do Sol no que diz respeito ao tratamento dos funcionarios 99% como positivo.





  
