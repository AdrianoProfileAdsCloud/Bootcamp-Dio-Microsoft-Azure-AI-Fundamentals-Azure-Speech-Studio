#Bootcamp Dio-Microsoft-Azure-Speech Studio.
Se trata de um projetinho de forma mais a nivel de apresentar o que foi aprendido no módulo Azure-Speech-Studio.Exploramos o uso do Azure Speech Studio e a análise linguística proporcionada pelo Language Studio.
"Aprofundei" o entendimento sobre como aproveitar essas ferramentas avançadas da Microsoft Azure. Tendo como foco aprimorar as habilidades na implementação de soluções de análise de fala e linguagem, o que proporcionou uma compreensão mais ampla e prática das capacidades oferecidas por essas tecnologias inovadoras.
A seguir vou realizando um passo a passo de como fiz essas implementações na prático no portal do Microsoft Azure.
Tendo como objetivo apenas mostrar meu entendimento. Tendo em vista que para tais passos que irei descrever abaixo e possível obter no site oficial da Microsoft.Aqui descrevo do meu modo, com base nos conhecimentos adquiridos nas aulas.

 ### Conversão de Audio em Texto.
 
Primeiro é preciso criar o Serviços Cognitivos.
Em seguida navegue para a página do Estúdio de fala em:
   https://speech.microsoft.com/, claro acessando com a mesa conta.

 Estando no Estudio de Fala seleciomos o idioma desejado.Em seguida escolhemos os arquivo(s) de audio a ser convertido(Conversão de fala em Texto.mp3). 
 
![Conversão de fala em Texto](https://github.com/AdrianoProfileAdsCloud/PRJ--Azure-Speech-Studio/blob/main/prints/Convers%C3%A3o%20de%20fala%20em%20Texto.jpg)

   Enão logo, será mostrado ao lado em Resultado de Teste a converão do audio para texto conforme o aúdio é executado.
   
![Exibição da Conversão de Fala em texto](https://github.com/AdrianoProfileAdsCloud/PRJ--Azure-Speech-Studio/blob/main/prints/Convers%C3%A3o%20de%20fala%20em%20Texto.jpg)

   Com este serviço é possivél converter qualquer audio em fala.Não só isso podemos fazer essa conversão do audio em qualquer idioma.
    No https://github.com/Azure-Samples/cognitive-services-speech-sdk ainda podemos ver com o sdk as implementações possíveis do serviço para algumas linguagens de programação e sistemas operacionais.

  ![Usando o Sdk do serviços de fala](https://github.com/AdrianoProfileAdsCloud/PRJ--Azure-Speech-Studio/blob/main/prints/Usando%20o%20Sdk%20do%20servi%C3%A7os%20de%20fala.jpg)
  
   Entre outras informações contidas ainda na mesma pagina do Estudio de fala - Conversação de fala em texo em tempo real.

   ![Proximas Etapas](https://github.com/AdrianoProfileAdsCloud/PRJ--Azure-Speech-Studio/blob/main/prints/Proximas%20Etapas.jpg)


### Análise de Sentimentos com Language Studio no Azure AI.
   
  Consiste em analise Semantica de texto ou fala;precisamente análise de sentimentos.Dando-se pelo processamento da Linguagem Narural(PNL).
  É o ramo da IA que nos ajuda na interpretação de mensages, textos e liguagens de uma forma geral.

   Para tal, já logado no portal seguiremos alguns passos:
    1- Criar um Recurso. 
    2- Selecionar - AI + Machine Learning.
    3- Selecionar - Language service.
    
   ![Analise de Sentimentos ](https://github.com/AdrianoProfileAdsCloud/PRJ--Azure-Speech-Studio/blob/main/prints/Analise%20de%20Sentimentos%20.jpg)
   
    Na tela a seguir mostrará as Defauts features.Seguimos clicando em: Continue to create your resource.
    
 ![criar idioma](https://github.com/AdrianoProfileAdsCloud/PRJ--Azure-Speech-Studio/blob/main/prints/criar%20idioma.jpg)
 
   Observação: Uma coisa muito importante que deverá ser lembrada a todo instente é o Uso Responsável da IA.
![UsoResponsavelIA](https://github.com/AdrianoProfileAdsCloud/PRJ--Azure-Speech-Studio/blob/main/prints/UsoResponsavelIA.jpg)

  Em seguida ao marcar o termo de uso Uso Responsável da IA. E só clicar e Revisar/criar
   A implantação do serviço começará.
   
   ![Processo de Implantação](https://github.com/AdrianoProfileAdsCloud/PRJ--Azure-Speech-Studio/blob/main/prints/Processo%20de%20Implanta%C3%A7%C3%A3o.jpg)
   
   Após o termino da implantação navegar para o Language Cognitive em:
    https://language.cognitive.azure.com/home.

   Obs: Em Resource name - Selecionar o resorce criado na etapa anterior.Para ser feito o link com o serviço a ser usado.
   
![languageCognitive](https://github.com/AdrianoProfileAdsCloud/PRJ--Azure-Speech-Studio/blob/main/prints/languageCognitive.jpg)

   Como queremos analisar através do texto selecionado o grau de safistação por exemplo de um cliente em resposta a um serviço oferecido. Devemos então selecionar - Classify text - Analyze sentiment mine options.
   
![Classify Text](https://github.com/AdrianoProfileAdsCloud/PRJ--Azure-Speech-Studio/blob/main/prints/Classify%20Text.jpg)

  Na próxima tela podemos trabalhar de duas formas:
   Entranos com o texto diretamente da área - Enter your own text, upload a file...
   Ou realizamos o upload do arquivo de texto que se deseja realizar a análise em - Arraste e solte arquivo(s)...
   
![language Studio](https://github.com/AdrianoProfileAdsCloud/PRJ--Azure-Speech-Studio/blob/main/prints/language%20Studio.jpg)

   ### Ao analisar o texto contido no arquivo de texto Analise-Restaurante.txt(na pasta inputs), é possivél de imediato ter a resposta se os serviços prestados em geral agradou de forma positiva ou negativa o cliente.

   ![Analise - Restaurante](https://github.com/AdrianoProfileAdsCloud/PRJ--Azure-Speech-Studio/blob/main/prints/Analise%20-%20Restaurante.jpg)

    Neste caso vemos após a analise que de forma geral o cliente ficou satifeito pois 78% correspponde que tudo ocorreu bem.
    Com uma parcela de 7% apenas dos serviços prestados estavam com algum problema.
    Tendo como Sentimento da frase(texto analisado, de acordo com o cliente) dado como positivo com confiaça de 94%.
     Manifestando a opinião sobre os pratos servidos com avaliações tido como deliciosos sinalando positividade.

   ### Ao analisar o texto contido no arquivo de texto Analise-Hotel.txt (na pasta inputs), é possivél de imediato ter a resposta se os serviços prestados em geral agradou de forma positiva ou negativa o cliente.

   ![Analise - Hotel](https://github.com/AdrianoProfileAdsCloud/PRJ--Azure-Speech-Studio/blob/main/prints/Analise%20-%20Hotel.jpg)

    Neste caso vemos após a analise que de forma geral o cliente ficou satifeito pois 96% correspponde que tudo ocorreu rasoavelmente bem nos na tratativa dos clientes.
    Com uma parcela de 3% corresponder como analise neutra.
    Tendo como Sentimento da frase(texto analisado, de acordo com o cliente) dado como positivo com confiaça de 96%.
     Manifestando a opinião sobre o Hotel Paríso do Sol no que diz respeito ao tratamento dos funcionarios 99% como positivo.





  
