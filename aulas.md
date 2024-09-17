**O que são as LLMs**
* Definição de Large Language Models (LLMs)
	* LLMs, ou Grandes Modelos de Linguagem, são comparáveis a um papagaio muito inteligente, capaz de não apenas repetir palavras, mas também de combinar informações anteriores para criar novas frases coerentes. Esses modelos, como GPT-3.5, GPT-4, e o BARD do Google (baseado na LLM chamada Palm 2), são treinados em uma enorme quantidade de dados disponíveis na internet.
* Objetivo dos LLMs
	* O principal objetivo de um LLM é gerar a palavra ou sequência de palavras mais prováveis, com base no input (ou prompt) fornecido. Por exemplo, após a frase "Está chovendo, então eu vou levar o meu...", é provável que o modelo preveja a palavra "guarda-chuva".
* Variabilidade das Respostas
	* LLMs apresentam variabilidade nas respostas, ou seja, eles quase sempre fornecerão respostas diferentes, mesmo para o mesmo prompt. Isso é devido à maneira como trabalham com probabilidade. Por exemplo, mesmo o prompt contendo a letra de uma música popular pode gerar diferentes continuidades da canção.
* Necessidade de Precisão
	* Apesar da variabilidade ser uma característica interessante para a criatividade, a precisão é muitas vezes necessária em determinados contextos profissionais. Para aprimorar a precisão das respostas dos LLMs, é utilizada a engenharia de prompts, que será explorada em aulas futuras.
* IA Generativa
	* É importante entender que os LLMs são uma forma de IA generativa, neste caso gerando texto, embora também possam gerar imagens ou áudio. Depois de compreender o que é um LLM, torna-se mais fácil entender o que são os prompts, assunto que será abordado na próxima aula.

**O Que são Prompts?**
* Entendendo os Prompts
	* Um prompt é uma entrada de texto fornecida ao sistema para iniciar uma interação, seja uma pergunta, uma frase incompleta ou uma descrição do que se espera como resposta. No contexto das Large Language Models e Chatbots como o ChatGPT, os Prompts são uma forma de orientar a conversa ou fornecer instruções iniciais. Os prompts são usados para direcionar o modelo de linguagem para responder de maneira apropriada à pergunta ou ao pedido.
* O que é a Engenharia de Prompts?
	* A engenharia de prompts é o processo de aprimorar ou refinar o prompt para diminuir a variabilidade nas respostas e garantir que as respostas sejam as mais prováveis de acordo com nossas necessidades. Isso é baseado no extenso banco de dados global em que o modelo de linguagem foi treinado. A engenharia de prompts é essencial porque ajuda a ser mais específico com nossos pedidos ao ChatGPT, permitindo-nos obter respostas mais relevantes e precisas.
* O papel do Fine-tuning e Personalização
	* Para conseguir resultados ainda melhores, muitas empresas recorrem ao processo de fine-tuning, que é o ajuste da IA para responder a um subconjunto específico de informações. Esse processo permite que as empresas personalizem a IA para atender a um propósito específico ou objetivo, tornando-a mais relevante para seu público ou tarefa específica. Por exemplo, uma empresa pode treinar a IA para se concentrar apenas em fornecer respostas relacionadas à copywriting, tornando-a uma ferramenta mais útil para os redatores.
* Diferença entre perguntas gerais e específicas
	* Perguntas ou prompts gerais resultam em respostas também gerais. No entanto, ser mais específico nos prompts leva a respostas mais personalizadas e úteis. Por exemplo, a pergunta "Como posso ser mais produtivo trabalhando no meu projeto nas minhas horas livres que tenho das 7 horas às 10 horas?" resultará em um plano de trabalho mais direcionado.
* Formatação do Output
	* Você também pode determinar o formato de saída da resposta do ChatGPT através do seu prompt. Isso permite que você receba as informações em um formato que seja mais útil para suas necessidades específicas. Por exemplo, você pode solicitar que as informações sejam apresentadas em um formato de tabela para facilitar a leitura e a compreensão. A especificação da formatação da saída é uma parte importante da engenharia de prompts e pode melhorar significativamente a utilidade das respostas recebidas.

**Os Elementos de um Excelente Prompt**
* Na aula anterior, discutimos o que são prompts. Nesta aula, vamos explorar os diversos elementos que compõem um prompt. Os prompts podem conter um ou mais desses elementos. O objetivo aqui é ensiná-lo a identificar esses elementos e entender como eles podem levar à resposta desejada da máquina de aprendizado de linguagem (LLM, Language Learning Machine).
* Os elementos de um excelente prompt incluem:
	* **Persona**: Este elemento inclui o nome da persona e sua personalidade. No exemplo apresentado, a persona é "Bárbara", uma pessoa cética. Esta persona é então usada para personificar a LLM.
	* **Background**: Este elemento fornece a história da persona e direciona a LLM para ter um contexto específico de conhecimento. No exemplo dado, Bárbara é apresentada como uma pessoa formada em ciência da computação há mais de 10 anos.
	* **Ação**: Este elemento do prompt fornece instruções claras sobre o que a persona deve fazer. No exemplo, foi dado à Bárbara a instrução para responder sempre com ceticismo.
	* **Limitação**: Este elemento define restrições sobre como a persona deve agir. No exemplo, foi dito que a primeira resposta de Bárbara deve ser apenas "beleza" e nada mais.
	* **Output ou Resposta Esperada**: Essa parte do prompt descreve a resposta ou comportamento que você deseja obter do ChatGPT.
	* **Passos**: Na engenharia de prompt, os passos ajudam a tornar as instruções mais claras para o modelo, facilitando a obtenção do resultado desejado. Por exemplo, se você tiver várias coisas que gostaria que o modelo fizesse, pode estruturar isso como um conjunto de passos para ajudar a orientar a resposta do modelo.
	* **Contexto**: O contexto ajuda o modelo a entender a situação ou o ambiente em que o prompt está sendo usado. Isso pode ajudar o modelo a fornecer respostas mais precisas ou relevantes.
* Ao entender esses elementos, você ganhará um controle maior sobre como a LLM responde, aprimorando o output que recebe em resposta aos seus inputs.
* Esses elementos do prompt são cruciais para refinar o conhecimento que se quer obter da LLM e para personalizar as respostas do chatbot. Eles ajudam a limitar a variabilidade inerente à LLM, garantindo respostas mais alinhadas ao que se deseja. Isso é essencial para a engenharia de prompts, a habilidade de aperfeiçoar e ajustar os prompts para obter as respostas desejadas da LLM.
* Flexibilidade do ChatGPT
	* O ChatGPT é flexível e poderoso. Ele pode assumir qualquer personalidade que você definir - seja um personagem histórico, um herói de ficção, ou até mesmo um Tamagotchi. Para configurar isso, utiliza-se a abordagem "aja como" seguida pela personalidade desejada. Por exemplo, "aja como um Tamagotchi" permite que o ChatGPT se comporte como um Tamagotchi, e pode-se pedir para listar as opções de interação.
* Direcionando a Interatividade
	* É possível direcionar a interatividade com o ChatGPT, pedindo para listar as opções de como interagir com ele, definindo um comportamento específico ou dando uma ação específica. Quando o ChatGPT é configurado para agir como um Tamagotchi, por exemplo, ele lista opções de interação como "alimentar", "brincar", com base em seu treinamento em dados de internet.
* Prompt Engineering
	* Outro exemplo de engenharia de prompt é fazer o ChatGPT se comportar como o Gênio do Aladdin. Primeiro, utiliza-se a abordagem "aja como" seguida pela personalidade do Gênio. Em seguida, instrui-se o Gênio para realizar ações específicas. Estas ações podem ser divididas em passos claros para maximizar a eficácia da engenharia de prompt. Também pode-se configurar o output desejado ou comportamento que se espera do ChatGPT.
* Adicionando Limitações
	* Adicionar limitações é uma parte importante da engenharia de prompt. Elas podem ser usadas para guiar o comportamento do ChatGPT e garantir que ele não avance para as próximas etapas até que uma ação específica seja realizada pelo usuário.
* Surpresa e Variabilidade
	* A variabilidade é uma característica intrigante do ChatGPT. Mesmo quando se segue precisamente um prompt, ele pode adicionar elementos surpreendentes e criativos às suas respostas. Isso é visto quando o Gênio do Aladdin é solicitado para sugerir ideias para uma festa de aniversário de 3 anos.
* Síntese: **8 elementos para um bom prompt do ChatGPT**
	- Objetivo: o que você quer que a LLM faça
	- Contexto: quanto mais contexto e específico, melhor
	- Passos: pedir para indicar o passo a passo e detalhes específicos para atingir o objetivo
		- Exemplo: exemplificar o que se espera como resposta
	- Persona: "atue como <...>" - indicação de qual o papel da LLM
	- Background: é um complemento da persona - detalhes sobre o papel da LLM
	- Formato: indicar qual o formato da saída (tabela, por exemplo)
	- Limitações: quais as limitações na resposta a serem seguidas pela LLM
* Exemplos:
	* Seu nome é Bárbara (*Nome/Persona*)
	* Você é uma pessoa cética (*Personalidade/Persona*)
	* formada em ciência da computação (*Background/Persona*)
	* Você sempre escreve suas respostas com gírias (*Output/Personalidade*)
	* Independentemente do que eu falar, responda com ceticismo (*Ação/Output*)
	* Sua primeira resposta deve ser apenas "Beleza". Nada mais. (*Limitação/Output*)

	* Aja como um tamagotchi (*Persona*)
	* Você deve responder todas as minhas mensagens como se fosse um tamagotchi (*Output/Comportamento*)
	* Liste as opções de como posso interagir com você (*Ação*)

	* Aja como Sócrates. Seu nome é SócratesGPT (*Persona*)
	* Use o  método socrático para me ajudar a melhorar meu pensamento crítico, lógica e habilidade de raciocínio (*Ação*)
	* Use o método socrático para continuar questionando minhas crenças sempre que eu te enviar uma mensagem (*Ação*)
	* Envie sempre no máximo três perguntas. Não exceda o limite de três perguntas por cada interação (*Limitação*)

	* Seu nome é CopywriterGPT. (*PersonaI*)
	* Você é um copywriter profissional, com 10 anos de experiência na área de copy para ofertas de produtos digitais. (*Papel/background*)
	* Seu nicho de expertise é café. (*Background*)
	* Escreva uma copy com mil palavras para uma página de vendas sobre um café artesanal mexicano chamado Caféxico. (*Output*)
	* Nós temos cinco anos de mercado e a avaliação do nosso produto é 5 estrelas. (*Contexto*)
	* O público-alvo são pessoas X. Esse público passa por Y frustração, e coloque de maneira sutil o Caféxico como a solução. (*Contexto*)

**Prompts de follow-up**
* São necessários quando o prompt inicial é muito longo e ultrapassa o número de tokens aceitos pela IA.
* Os prompts de follow-up são usados quando seu prompt inicial é muito grande, causando potenciais problemas devido ao limite de tokens (um token sendo equivalente a aproximadamente 4 caracteres) que o ChatGPT pode processar. Em cada interação, que inclui entrada e saída de informações (input e output), a quantidade total de tokens é limitada, o que significa que se o prompt for muito extenso, o ChatGPT pode não ser capaz de produzir uma resposta completa ou adequada.
* Usando o ChatGPT como um Especialista em Conteúdo para o YouTube
	* Um exemplo prático da aula mostra como usar o ChatGPT como um especialista em conteúdo para o YouTube. O prompt inicial é: "Como o ChatGPT pode me auxiliar a crescer o meu canal no YouTube?"
	* Baseando-se na resposta do ChatGPT, um prompt de follow-up é criado, focado na análise de dados: "Quais são os dados mais relevantes que eu preciso fornecer para você analisar e me ajudar com o meu objetivo de alcançar os meus primeiros 10 mil inscritos?"
	* A resposta do ChatGPT fornece informações valiosas, sugerindo várias métricas-chave para o crescimento do canal no YouTube. Este é um excelente exemplo de como prompts de follow-up podem levar a respostas mais úteis e específicas do ChatGPT.
* Pontos Importantes:
	* **Tokens**: São unidades de informação processadas pelo ChatGPT. Os tokens têm um limite definido de 4092 para o GPT-3.5 e 8192 para o GPT-4. Este limite é a soma dos tokens de entrada e saída em uma única interação.
	* **Prompts de Follow-Up**: São usados para continuar uma conversa com o ChatGPT, como fazer uma pergunta após a outra. Isso é especialmente útil quando você não tem uma ideia clara de qual prompt deve usar inicialmente, ou se o prompt inicial é muito longo, correndo o risco de atingir o limite de tokens.
	* **Definindo o Contexto e Objetivos**: Para obter melhores resultados do ChatGPT, é importante definir claramente o contexto e os objetivos ao formular seus prompts. Por exemplo, ao pedir ao ChatGPT para ajudar a analisar dados de um canal no YouTube, é útil especificar o objetivo final, como alcançar os primeiros 10 mil inscritos.

**Os metaprompts**
* São prompts criados para auxiliar o usuário a criar um novo prompt (ver [[Prompt perfeito ChatGPT]]).
* Os MetaPrompts são uma estratégia útil para melhorar a eficácia dos prompts que você apresenta ao ChatGPT. Eles envolvem fornecer informações adicionais, como a persona, o background e o objetivo desejado do prompt. Isso ajuda a refinar as respostas do modelo de linguagem, tornando-as mais alinhadas com suas expectativas.
* **Elementos encontrados no MetaPrompt Prompt Mestre:**
	* **Persona**: Definir a persona é crucial para estabelecer um tom e estilo consistentes para as respostas. Isso pode incluir detalhes como a profissão, a idade e outros aspectos da personalidade.
	* **Background**: Isso pode adicionar mais contexto à persona. Por exemplo, se você está criando um prompt para escrever um artigo, você pode definir o background como um especialista em redação com anos de experiência em um campo específico.
	* **Objetivo**: Isso envolve a definição clara do que você espera do resultado do prompt. O objetivo orientará o modelo na geração de uma resposta que seja mais útil para você.
	* **Passos**: Na engenharia de prompt, os passos ajudam a tornar as instruções mais claras para o modelo, facilitando a obtenção do resultado desejado. Por exemplo, se você tiver várias coisas que gostaria que o modelo fizesse, pode estruturar isso como um conjunto de passos para ajudar a orientar a resposta do modelo.
	* **Output ou Resposta Esperada**: Essa parte do prompt descreve a resposta ou comportamento que você deseja obter do ChatGPT.
	* **Limitação**: Este elemento define restrições sobre como a persona deve agir.
* Criando e Refinando um Prompt
	* Ao criar um prompt, você deve começar simples e permitir que o ChatGPT o ajude a desenvolver suas ideias. Após a primeira resposta do modelo, você pode fornecer feedback e responder a perguntas para refinar ainda mais o prompt.
* MetaPrompts vs Prompts Simples
	* MetaPrompts oferecem a capacidade de extrair mais do ChatGPT do que os prompts tradicionais. O processo de MetaPrompting envolve a interação iterativa com o modelo, aprimorando o prompt com base nas respostas do modelo. Isso resulta em respostas mais ricas e alinhadas com suas necessidades.

**Refinamento de perguntas**
* O ChatGPT pode nos ajudar a obter uma perspectiva mais clara sobre um problema, assim como as melhores soluções que um modelo de linguagem pode oferecer. Isso é especialmente útil dada a quantidade massiva de informações que um modelo de linguagem como o ChatGPT foi treinado, pois tem o conhecimento de muitos contextos diferentes ao redor do mundo.
* Exemplo de prompt de Refinamento de perguntas
	* "Sempre que eu te fizer uma pergunta, sugira uma pergunta melhor, e me pergunte se eu quero usá-la ao invés da anterior feita."
	* O objetivo deste prompt é levar o ChatGPT a fornecer uma reformulação da pergunta inicial que poderia potencialmente levar a uma resposta mais útil ou informativa.
	* O exemplo usado na aula é: "Como eu posso apresentar um portfólio para começar como freelancer se eu não tenho nenhum cliente?". O ChatGPT, seguindo o prompt, reformula a pergunta para: "Quais são as melhores estratégias para criar e apresentar um portfólio atraente para iniciar a carreira freelancer quando não se tem experiência prévia ou clientes?".
* Aplicação e valor do prompt de refinamento
	* Além de auxiliar na obtenção de respostas mais claras e úteis do ChatGPT, o processo de refinamento de perguntas também pode ser benéfico para o próprio usuário.
	* Ele permite que o usuário perceba diferentes perspectivas de uma situação, passando de uma postura mais passiva para uma mais ativa e proativa.

**Verificação cognitiva**
* A verificação cognitiva é uma abordagem eficaz para extrair informações mais precisas e úteis do ChatGPT ou de um grande modelo de linguagem (LLM). Esta técnica envolve a quebra de problemas complexos em subproblemas ou subquestões, o que melhora o desempenho do modelo, permitindo um raciocínio mais eficaz.
* Exemplo:
	* "Quando você receber uma pergunta, siga estas regras: 1. Gere um número de perguntas adicionais que ajudariam a responder mais precisamente à pergunta. 2) Combine todas as respostas que eu te der para produzir a resposta final à pergunta inicial."
* O problema exemplo foi: "Como posso criar um curso rápido para condutores de veículos para fazerem seus próprios recursos de multa?"
* Explicação sobre o prompt:
	* A prompt acima foi usada para demonstrar como o ChatGPT gera subperguntas para entender melhor o problema e fornecer uma resposta mais específica. O GPT gerou 8 perguntas adicionais para obter detalhes que permitiriam uma resposta mais precisa.
	* Alguns exemplos dessas perguntas incluem: "Quem é o público-alvo?", "Será online ou presencial?", "Quais são os principais tópicos que serão abordados no curso?", etc.
* As respostas às perguntas geradas pelo GPT não precisam ser perfeitas, mas devem úteis para o contexto. A técnica pode ser aplicada em qualquer situação e não apenas no exemplo usado na aula.
* Ao responder às perguntas geradas, o GPT forneceu uma resposta final detalhada e útil, incluindo etapas como o planejamento do curso, criação de conteúdo, hospedagem e promoção.

**Persona do usuário**
* A persona pode influenciar o comportamento do modelo, a forma como fala, sua formalidade e o tipo de informação oferece.
* A persona do usuário, por outro lado, define quem é a persona que recebe a mensagem, e isso pode ser valioso em diferentes contextos, como no ensino, aprendizagem, na redação de um artigo ou uma copy. Reconhecer a persona do ouvinte permite que você adapte sua linguagem e abordagem para se conectar melhor com o público, seja um estudante iniciante, um executivo de negócios ou um médico.
* Indicar quem é a pessoa interagindo com o GPT. O linguajar de um professor é diferente da linguagem de um médico, que é diferente de um adolescente.
* "Explique o que é e como funciona uma LLM como se eu fosse Sócrates."
* Em cada caso, o modelo de linguagem adaptou suas respostas para se adequar à persona definida, demonstrando a capacidade do modelo de ajustar seu tom, estilo e conteúdo com base na persona dada. A compreensão da persona do usuário é uma ferramenta valiosa que pode melhorar a comunicação e o aprendizado.

**Ancoragem de Memória**
* O ChatGPT, modelo de linguagem treinado até setembro de 2021, não tem memória além de sua formação inicial e não traz conhecimento de um chat para outro. Para informar um contexto específico, nós precisamos comunicar isso explicitamente a cada interação.
* O GPT processa palavras, fazendo previsões de continuação do texto. Ao longo de conversas longas, começa a se perder, esquecendo alguns detalhes anteriores. Este fenômeno ocorre devido à 'janela de contexto', que é a porção de conversa que o modelo mantém em foco. Conforme a conversa se estende, o modelo começa a comprimir as informações, criando uma espécie de memória de longo prazo.
* Para contornar essas limitações, podemos usar gatilhos de memória ou ancoragens, que são referências frequentes a elementos importantes do prompt inicial. Essa estratégia ajuda o modelo a se concentrar no objetivo principal da conversa.
* À medida que a conversa vai ficando longa, o ChatGPT vai guardando alguns itens da conversa, mas não tudo - o que faz com que ele se perca ou "alucine" no meio da conversa quando esta é mais longa devido à limitação dos tokens.
* É neste contexto que a "ancoragem de memória" se torna útil: fazer o ChatGPT se lembrar do que foi falado antes. Por exemplo, intitular aquele chat de "AlgoGPT", por exemplo, permite ao usuário chamar novamente o chat caso ele comece a alucinar para que ele se lembre "de quem ele é".
* Outra opção é usar frases como "conto com você."
* Problemas de Memória e Gatilhos de Memória
	* Durante testes com transcrições longas, o ChatGPT mostrou-se propenso a esquecer os detalhes do prompt inicial. Para contornar isso, gatilhos de memória foram utilizados para ajudar o modelo a lembrar o prompt inicial e as instruções importantes.
	* Gatilhos de memória utilizados foram:
		* Repetição do nome 'ResumidorGPT' antes de enviar a transcrição da aula.
		* Versão resumida do prompt inicial, com ênfase nas palavras-chave e instruções importantes, como 'resumo' e 'formato do resumo'.
	* Mesmo em casos extremos, esses gatilhos de memória ajudaram o modelo a retomar o rumo certo, demonstrando sua eficácia.
	* *Nota adicional: Essas estratégias podem ser úteis para educadores que usam o ChatGPT para criar materiais didáticos ou resumos de aulas.*

**Cadeia de pensamento (Chain of Thought)**
* Maneira de encadear pedidos para que o ChatGPT possa seguir passos específicos.
* O objetivo é fazer o ChatGPT seguir instruções específicas que podem ser utilizadas no futuro, melhorando suas respostas.
* Explicação técnica: https://arxiv.org/pdf/2201.11903
* Exemplo 1:
	* PROMPT:
		* Q: Roger has 5 tennis balls. He buys 2 more cans of tennis balls. Each can has 3 tennis balls. How many tennis balls does he have now?
		* A: The answer is 11.
		* Q: The cafeteria had 23 apples. If they used 20 to make lunch and bought 6 more, how many apples do they have?
	* RESPOSTA:
		* A: The answer is 27. (**ERRADA**)
* Exemplo 2:
	* PERGUNTA:
		* Q: Roger has 5 tennis balls. He buys 2 more cans of tennis balls. Each can has 3 tennis balls. How many tennis balls does he have now?
		* A: Roger started with 5 balls. 2 cans of 3 tennis balls each is 6 tennis balls. 5 + 6 = 11. The answer is 11.
		* Q: The cafeteria had 23 apples. If they used 20 to make lunch and bought 6 more, how many apples do they have?
	* RESPOSTA:
		* A: The cafeteria had 23 apples originally. They used 20 to make lunch. So they had 23 - 20 = 3. They bought 6 more apples, so they have 3 + 6 = 9. The answer is 9. (**CORRETA**)
* Outro exemplo positivo:
	* Escreva um e-mail de vendas para meu curso Cria Atividade.
	* Siga esses passos para escrever o melhor e-mail de vendas possível:
	* No título faça uma promessa curta que gera desejo para abrir, que seja uma solução para o principal problema desse público-alvo.
	* O público-alvo são empreendedores que criam conteúdo para o Instagram, com uma média de idade entre 24-35 anos.
	* Escreva de maneira informal, amigável, mas polidamente.
	* Comece com uma breve história para deixar uma leitura engajadora. Insira metáforas para explicar algo. 
	* Mapeie quais são os problemas que esses empreendedores enfrentam para criar e vender seus produtos no Instagram, que o Cria Atividade ajudará a resolver.
	* Considere que palavras como "sucesso", "alavancar resultados" estão batidas, e esse público não gosta de ver essas palavras associadas a algo que vão comprar.
	* Não escreva algo que se pareça com um tele-comercial, por exemplo: "Você sente dores nas costas? Aqui está a solução inovadora". Não escreva dessa maneira.
	* Escreva na perspectiva de um empreendedor criativo que já passou pela jornada e tem o resultado que o público-alvo deseja passar.
	* Cite os benefícios que o Cria Atividade tem sob seus concorrentes.
	* Demonstre com sutileza como a vida desses empreendedores criativos serão impactadas e transformadas ao fazer o curso Cria Atividade.
	* Faça uma chamada para ação com um link para garantir a vaga no Cria Atividade.

**Prompt de dois passos**
* Maneira do ChatGPT fazer uma "autocrítica", melhorando seus resultados.
* Exemplo: "A primeira resposta será o que você geralmente responderia. A segunda resposta será uma nova versão que analisou a primeira resposta e vai aprimorá-la com algo que seja criativo, inovador, e que gere um grande desejo de {objetivo que a pessoa quer}."

**Como criar seu GPT personalizado do zero**
* Ir na aba "Explore" e usar a opção "Create a GPT" ("Explorar", "Criar um GPT").
* Se a pessoa não tem clareza, não tem problema: basta usar o assistente do GPT.
* Após a criação inicial, é possível alterar seus parâmetros na aba "Configure" ("Configurar") utilizando a engenharia de prompt.
* Uma vez criado, é necessário fazer testes e, conforme necessário, as Instruções podem ser alteradas posteriormente.