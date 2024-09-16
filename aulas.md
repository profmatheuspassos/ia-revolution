**8 elementos para um bom prompt do ChatGPT**
- Objetivo: o que você quer que a LLM faça
- Contexto: quanto mais contexto e específico, melhor
- Passos: pedir para indicar o passo a passo e detalhes específicos para atingir o objetivo
- Exemplo: exemplificar o que se espera como resposta
- Persona: "atue como <...>" - indicação de qual o papel da LLM
- Background: é um complemento da persona - detalhes sobre o papel da LLM
- Formato: indicar qual o formato da saída (tabela, por exemplo)
- Limitações: quais as limitações na resposta a serem seguidas pela LLM

Exemplo:
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

**Os metaprompts**
* São prompts criados para auxiliar o usuário a criar um novo prompt (ver [[Prompt perfeito ChatGPT]]).

**Refinamento de perguntas**
* "Sempre que eu te fizer uma pergunta, sugira uma pergunta melhor baseada na minha pergunta, e me pergunte se eu quero usá-la ao invés da minha pergunta original."

**Verificação cognitiva**
* "Quando você receber uma pergunta, siga estas regras: 1. Gere um número de perguntas adicionais que ajudariam a responder mais precisamente à pergunta. 2) Combine todas as respostas que eu te der para produzir a resposta final à pergunta inicial."

**Persona do usuário**
* Indicar quem é a pessoa interagindo com o GPT. O linguajar de um professor é diferente da linguagem de um médico, que é diferente de um adolescente.
* "Explique o que é e como funciona uma LLM como se eu fosse Sócrates."