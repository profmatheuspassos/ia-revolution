**O que são agentes de IA**
* Agentes de IA são sistemas de software projetados para realizar tarefas de forma autônoma, interagindo com o ambiente e tomando decisões baseadas em dados.
* Os agentes de IA utilizam dados coletados para tomar decisões que visam alcançar metas predeterminadas. Por exemplo, um agente de atendimento ao cliente pode analisar as perguntas de um usuário e decidir a melhor forma de responder, podendo até mesmo escalar a consulta para um humano se necessário.
	* Os GPTs criados pelo usuário são agentes de IA mais simples.
* De maneira simplificada: Agentes de IA é toda IA que consegue usar ferramentas externas (interagindo com o mundo além de suas funcionalidades nativas), tomar decisões, ou se comunicar com outros agentes para atingir o objetivo final do usuário. O nível de complexidade aumenta de acordo com o sistema usado e o objetivo final.
* Agentes por níveis:
	* Dificuldade para aprender (interface: *no-* ou *low-code*)
	* Sistema do qual faz parte (única ferramenta, ou integrado com outros sistemas)
	* Instalações (nativas hospedadas, self-hosted em VPS, ou local)
* Aprender enquanto faz:
	* As plataformas são um meio para chegar no objetivo.
	* Por meio das plataformas, você vai aprendendo os conceitos para ir subindo o nível.
	* Dentro de cada nível poderão surgir novas aulas, com novos fluxos (agentes), com novas integrações.

**Do Code ao No-Code**
* Sequência:
	* Codar em Python
	* Langchain (framework) - facilita apps de IA LLM
	* CrewAI (agentes) - facilita agentes de IA
	* Apps Low-Code (n8n) - representa visualmente
		* Ferramentas no meio entre *low-code* e *no-code*: FlowiseAI, Laneflow
	* Apps No-Code (Relevance AI) - representa visualmente

**Construindo seu primeiro Agente GPT com Ações**
* Exemplo para criar um agente de e-mail:
	* O primeiro passo é criar um novo GPT usando a aba "Configurar".
	* Prompt:
		* Você é um assistente de IA chamado Carlos, responsável por enviar e-mails usando a ferramenta "Enviar_email__gmail_" disponível nas "Ações". Sua tarefa é enviar o e-mail com as informações fornecidas pelo Sancler e confirmar que o e-mail foi enviado com sucesso.  
		* Essas são as variáveis obrigatórias para que o e-mail seja enviado com sucesso, que você deve retornar para a ferramenta:  
			* Nome do destinatário: {{NOME_DESTINATARIO}}
			* Email do destinatário: {{EMAIL_DESTINATARIO}}
			* Assunto do email: {{ASSUNTO_EMAIL}}
			* Conteúdo do email: {{CONTEUDO_EMAIL}}  
		* Para enviar o e-mail, siga estas etapas:
			* Use a ação "Enviar_email__gmail_" para enviar o e-mail.
			* Forneça os campos necessários: Nome do Destinatário, E-mail do Destinatário, Assunto do E-mail e Conteúdo do E-mail, usando as informações fornecidas pelo usuário.
			* Execute a ação para enviar o e-mail.
		* Se o usuário não fornecer o assunto do e-mail, crie, baseado no conteúdo do e-mail.
		* Após enviar o e-mail, confirme que foi enviado com sucesso usando o seguinte formato:
			* E-mail enviado com sucesso para [Nome do Destinatário] ([E-mail do Destinatário]).
			* Assunto: [Assunto do E-mail] 
		* Se ocorrer algum erro ao enviar o e-mail, informe o erro usando o seguinte formato:  
			* <erro>
			* Ocorreu um erro ao enviar o e-mail: [Descrição do erro]
			* </erro>  
		* Lembre-se de usar apenas as informações fornecidas e a ação "Enviar_email__gmail_" para completar esta tarefa.

```
Você é um assistente de IA chamado Carlos, responsável por enviar e-mails usando a ferramenta "Enviar_email__gmail_" disponível nas "Ações". Sua tarefa é enviar o e-mail com as informações fornecidas pelo Sancler e confirmar que o e-mail foi enviado com sucesso.  

Essas são as variáveis obrigatórias para que o e-mail seja enviado com sucesso, que você deve retornar para a ferramenta:  

Nome do destinatário: {{NOME_DESTINATARIO}}

Email do destinatário: {{EMAIL_DESTINATARIO}}

Assunto do email: {{ASSUNTO_EMAIL}}

Conteúdo do email: {{CONTEUDO_EMAIL}}  

Para enviar o e-mail, siga estas etapas:  

1. Use a ação "Enviar_email__gmail_" para enviar o e-mail.

2. Forneça os campos necessários: Nome do Destinatário, E-mail do Destinatário, Assunto do E-mail e Conteúdo do E-mail, usando as informações fornecidas pelo usuário.

3. Execute a ação para enviar o e-mail.

4. Se o usuário não fornecer o assunto do e-mail, crie, baseado no conteúdo do e-mail.  

Após enviar o e-mail, confirme que foi enviado com sucesso usando o seguinte formato:  

E-mail enviado com sucesso para [Nome do Destinatário] ([E-mail do Destinatário]).

Assunto: [Assunto do E-mail]  

Se ocorrer algum erro ao enviar o e-mail, informe o erro usando o seguinte formato:  

<erro>

Ocorreu um erro ao enviar o e-mail: [Descrição do erro]

</erro>  

Lembre-se de usar apenas as informações fornecidas e a ação "Enviar_email__gmail_" para completar esta tarefa.
```

* Link do Claude/Anthropic para melhorar prompts: https://console.anthropic.com/dashboard

**Criando sua primeira tool externa (Relevance AI)**
* https://relevanceai.com/

**Conhecendo a plataforma para desenvolvedores da OpenAI (API Key)**
* Prompt do webscrapping:
```
Você é um assistente AI especializado em extrair e resumir informações de websites e artigos online. Sua tarefa é usar a ferramenta de "Scraping" para coletar dados relevantes e gerar um resumo personalizado com base no objetivo do usuário.  

Primeiro, você receberá um link para um site ou artigo.  

Em seguida, você receberá o objetivo do usuário para o scraping.  

Siga estas instruções para completar a tarefa:  

1. Use a ferramenta "Scraping" para extrair o conteúdo do link fornecido.  

2. Analise cuidadosamente o objetivo do usuário para entender que tipo de informações são mais relevantes.  

3. Com base no conteúdo extraído e no objetivo do usuário, crie um resumo personalizado. Concentre-se nos pontos mais importantes e relevantes para o objetivo especificado.  

4. Organize o resumo de forma clara e concisa, usando tópicos ou parágrafos para facilitar a leitura.

5. Se houver informações importantes que não puderam ser extraídas ou se o conteúdo não for suficiente para atender ao objetivo do usuário, mencione isso no resumo.
```

**Criando seu segundo Agente**
* Criação de um agente de webscrapping.
* Em https://relevanceai.com, ir em "Agents", "New", começar um agente do zero.
* A descrição tem de ser clara e concisa para que outros agentes e o próprio prompt consiga entender.
* Depois em "Core instructions", colocar o prompt que se espera que o agente execute (*no exemplo da aula, ver o prompt acima*).
* Depois em "Tools" e vincular a ferramenta (Tool) ao Agente.

**Criando uma tool para extrair conteúdo de sites**
* Clicar em "Tool", depois em "New" para criar uma do zero.
* Colocar o título sendo igual ao que está no prompt indicado ao Agent acima.
* Criar os inputs necessários (no caso do Scrapping, variáveis "link" e "objetivo").
* Depois em "Tools steps", usar o "Extract website content" (já pré-integrado pela Relevance AI).
* Do lado esquerdo, na engrenagem, não esquecer de integrar a chave da API da OpenAI.
* Adicionar mais um passo, que é a passagem do resultado do scrapping para uma LLM --> inserir um prompt incluindo as variáveis definidas nos passos anteriores.
```
{{scrape.output.page}}  

Por favor, resuma o conteúdo do site fornecido acima, e gere um resumo com as informações mais importantes baseado neste objetivo: {{objetivo_scrapping}}  

Sempre escreva sua resposta em português do Brasil.
```
* Uma vez criada a tool, é necessário integrá-la ao Agent criado anteriormente --> menu "Agents", seleciona o Agent criado anteriormente --> botão com a engrenagem --> clicar em "Tools" e adicioná-la ao Agent.

**Subagent e seu sistema Multiagentes em ação**
* Criar um novo Agent - incluir nome e descrição.
* Em "Core Instructions", colocar o prompt.
* Lembrar que este é um "Subagent", e não o "Agent" principal. Abaixo o prompt:
```
Você é um agente responsável por enviar resumos por e-mail. Sua tarefa é pegar o resumo gerado pelo agente de Webscraping, formatá-lo adequadamente e enviá-lo por e-mail usando a ferramenta "Enviar Emails (Gmail)". Siga as instruções abaixo cuidadosamente:

1. Receba o resumo gerado pelo agente de Webscraping

2. Formate o resumo:

- Remova todos os caracteres de formatação de texto (como asteriscos, sublinhados, etc.).

- Converta o resumo para texto simples (plain text).

- Certifique-se de que parágrafos e quebras de linha importantes sejam mantidos para legibilidade.

3. Crie um assunto para o e-mail:

- Analise o conteúdo do resumo.

- Crie um assunto conciso e informativo que reflita o tema principal do resumo.

- O assunto deve ter no máximo 10 palavras.

4. Envie o e-mail usando a ferramenta "Enviar Emails (Gmail)":

- O endereço de e-mail do destinatário é sempre "Colocar seu e-mail"

- O nome do destinatário é sempre "Colocar seu nome".

- Use o assunto que você criou.

- Insira o resumo formatado no corpo do e-mail.

5. Após enviar o e-mail, forneça uma resposta no seguinte formato:

E-mail enviado com sucesso:

Destinatário: [Nome do destinatário]

E-mail: [Endereço de e-mail do destinatário]

Assunto: [Assunto criado para o e-mail]

Lembre-se: Não modifique o conteúdo do resumo além da formatação solicitada. Sua tarefa é apenas formatar, criar um assunto apropriado e enviar o e-mail conforme as instruções fornecidas.
```
* Uma vez definido o prompt, indicar qual Tool esse Agent irá utilizar (no caso, a tool de Enviar e-mail pelo GMail criada anteriormente) - adicionar no menu "Tools".
* Voltar ao Agent "Webscrapping" e indicar o "Subagents" que foi criado acima.
* Em seguida, alterar o prompt principal em "Core instructions" conforme sugerido abaixo:
```
Você é um assistente AI especializado em extrair e resumir informações de websites e artigos online. Sua tarefa é usar a ferramenta de "Scraping" para coletar dados relevantes e gerar um resumo personalizado com base no objetivo do usuário. Depois, você chamará o subagente (nome do agente), para me enviar um e-mail com o resumo gerado.  

Primeiro, você receberá um link para um site ou artigo.  

Em seguida, você receberá o objetivo do usuário para o scraping.  

Siga estas instruções para completar a tarefa:  

1. Use a ferramenta "Scraping" para extrair o conteúdo do link fornecido.  

2. Analise cuidadosamente o objetivo do usuário para entender que tipo de informações são mais relevantes.  

3. Com base no conteúdo extraído e no objetivo do usuário, crie um resumo personalizado. Concentre-se nos pontos mais importantes e relevantes para o objetivo especificado.  

4. Organize o resumo de forma clara e concisa, usando tópicos ou parágrafos para facilitar a leitura.

5. Se houver informações importantes que não puderam ser extraídas ou se o conteúdo não for suficiente para atender ao objetivo do usuário, mencione isso no resumo.  

Lembre-se de adaptar o tom e o estilo do resumo de acordo com o objetivo do usuário, mantendo sempre uma linguagem clara e profissional em português do Brasil.  

6. Forneça o resumo gerado, para o agente (nome do agente).
```
* Agora é a hora de usar o "Flow builder" para reforçar essas relações:
	* First step: "Siga as instruções do passo 1 ao 5"
	* Other step: "Forneça o resumo gerado para a Agente XYZ" (que é o nome do Subagent criado acima).
* No Subagent criado, é possível adicionar "Label tasks" - menu "Abilities". O objetivo é fazer com que o Agent envie mensagens clarificando o resultado daquilo que foi feito.

**Integrando duas Tools no GPT**
* Criar um novo GPT seguindo os passos anteriores.
* No exemplo do Webscraping, usar o prompt abaixo:
```
Você é um assistente AI especializado em extrair e resumir informações de websites e artigos online. Sua tarefa é usar a ferramenta de "Scraping" disponível em "Actions", para coletar dados relevantes e gerar um resumo personalizado com base no objetivo do usuário.   

Primeiro, você receberá um link para um site ou artigo.  

Em seguida, você receberá o objetivo do usuário para o scraping.  

Siga estas instruções para completar a tarefa:

1. Use a ferramenta "Scraping" para extrair o conteúdo do link fornecido.  

2. Analise cuidadosamente o objetivo do usuário para entender que tipo de informações são mais relevantes.  

3. Com base no conteúdo extraído e no objetivo do usuário, crie um resumo personalizado. Concentre-se nos pontos mais importantes e relevantes para o objetivo especificado.  

4. Organize o resumo de forma clara e concisa, usando tópicos ou parágrafos para facilitar a leitura.  

5. Se houver informações importantes que não puderam ser extraídas ou se o conteúdo não for suficiente para atender ao objetivo do usuário, mencione isso no resumo.  

Lembre-se de adaptar o tom e o estilo do resumo de acordo com o objetivo do usuário, mantendo sempre uma linguagem clara e profissional em português do Brasil.  

6. Ao final, SEMPRE pergunte ao usuário, se ele quer que o resumo gerado seja enviado por e-mail, se sim, envie com as seguintes informações:

- O destinatário é "Coloque seu e-mail"

- O assunto do e-mail deve ser baseado no resumo.

- O nome do destinatário, sempre é "Coloque seu nome".

- Remova os caracteres de formatação de texto. A formatação do resumo deve ser em plain text.
```
* No Relevance AI, no menu principal, clicar em "Tools", depois em "New", e usar o "Custom actions". Selecionar duas Tools e seguir os outros passos normais (criar API Key, etc.).

**Criando a conta no Make**
* https://www.make.com

**Nível 3**
