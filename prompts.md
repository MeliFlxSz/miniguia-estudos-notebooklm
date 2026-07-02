# Engenharia de Prompts e "Cicatrizes"

## Prompt 1

### Objetivo
Ter um primeiro contato com o assunto em questão.

### Prompt
Explique o ataque.

### Resultado
Os invasores criaram um site falso que imitava a página oficial do Claude para distribuir o malware PlugX (RAT). A vítima baixava um instalador aparentemente legítimo, que executava o aplicativo Claude real para não levantar suspeitas enquanto instalava, em segundo plano, o malware. O ataque utilizava a técnica de DLL sideloading para carregar a carga maliciosa, que estabelecia comunicação com um servidor de Comando e Controle (C2), concedendo acesso remoto ao computador. Além do roubo de credenciais e do registro de teclas digitadas, o malware apagava vestígios da instalação para dificultar a investigação. Como medida de proteção, recomenda-se baixar o Claude apenas pelo site oficial.

### Considerações
-A resposta foi organizada em tópicos, o que facilitou a leitura.
-As informações ficaram um pouco dispersas, dificultando a compreensão da sequência cronológica do ataque.
-Alguns conceitos técnicos (como DLL sideloading e servidor de Comando e Controle) foram apenas mencionados, sem aprofundamento.
-A resposta apresentou uma boa visão geral, mas poderia detalhar melhor como cada etapa do ataque se relaciona com a seguinte.
---

## Prompt 2

### Objetivo
Explorar a técnica da utilização de contextualização no prompt, a fim de conduzir o raciocínio em torno de um cenário específico (quem está ouvindo a explicação)

### Prompt
explique o ataque, considerando que a explicação está sendo feita para uma pessoa que está começando a ter contato com cibersegurança e não conhece os conceitos e termos da área.

### Resultado
Os criminosos criaram um site falso do Claude para enganar usuários e distribuir o malware PlugX. A vítima instala um programa que parece legítimo e até abre o Claude verdadeiro, mas, em segundo plano, o malware é instalado silenciosamente. Para evitar detecção, os invasores usam a técnica de DLL sideloading, fazendo um programa confiável carregar um arquivo malicioso. Depois disso, o PlugX abre uma porta dos fundos no computador, permitindo aos hackers roubar senhas, registrar teclas digitadas, acessar arquivos e controlar a máquina remotamente. O malware ainda apaga rastros da instalação para dificultar a investigação. A principal forma de prevenção é baixar o Claude apenas pelo site oficial e desconfiar de sites e arquivos suspeitos.

### Considerações
-A resposta passou a utilizar analogias e exemplos, tornando o conteúdo mais acessível para leitores iniciantes.
-A simplificação facilitou a compreensão geral do ataque, mas reduziu o nível de detalhamento técnico.
-Houve menor uso de termos técnicos, o que deixou o texto mais enxuto, porém menos preciso para um público especializado.
-O foco passou da descrição técnica para uma explicação didática do funcionamento do ataque.
---

## Prompt 3

### Objetivo
Explorar a técnica de delimitação de resposta, esclarecendo qual o direcionamento de resposta não é alinhado ao esperado.

### Prompt
explique o ataque, considerando que a explicação está sendo feita para uma pessoa que está começando a ter contato com cibersegurança e não conhece os conceitos e termos da área. Entretanto, apesar de ser iniciante em cibersegurança, a pessoa precisa entender de forma um pouco mais técnica e aprofundada, visto que ela é universitária de t.i. e ela precisa fazer uma apresentação desse estudo de caso, portanto não deve prevalecer simplificações e o uso de analogias durante todo o corpo do texto, sem esquecer de se apronfundar na explicação das terminologias próprias da área de cibersegurança

### Resultado
Este estudo de caso descreve uma campanha de phishing que utiliza engenharia social para distribuir o PlugX, um Trojan de Acesso Remoto (RAT). Os invasores criam um site falso do Claude e induzem a vítima a instalar uma versão inexistente do programa. Enquanto o aplicativo legítimo é executado para não despertar suspeitas, um dropper instala o malware e garante sua persistência ao copiá-lo para a pasta de inicialização do Windows. Em seguida, o ataque utiliza a técnica de DLL sideloading, fazendo um executável legítimo carregar uma DLL maliciosa, que descriptografa e executa o PlugX na memória. Após a infecção, o malware estabelece comunicação com um servidor de Comando e Controle (C2), permitindo acesso remoto, roubo de credenciais e registro de teclas digitadas. Para dificultar a investigação, o malware apaga vestígios da instalação e suprime mensagens de erro.

### Considerações
-A resposta assumiu que o leitor já possui conhecimentos básicos de cibersegurança, deixando alguns termos sem explicação.
-O foco passou a ser o funcionamento técnico do ataque, em vez de detalhar a narrativa do incidente.
-Houve maior aprofundamento nas técnicas utilizadas pelos invasores, com menor ênfase no contexto e na cronologia do caso.
---

## Prompt 4

### Objetivo
Utilizar do recurso de especificação do formato de saída e de exemplificação de qual formato objetivo.

### Prompt
explique o ataque, considerando que a explicação está sendo feita para uma pessoa que está começando a ter contato com cibersegurança e não conhece os conceitos e termos da área. Entretanto, apesar de ser iniciante em cibersegurança, a pessoa precisa entender de forma um pouco mais técnica e aprofundada, visto que ela é universitária de t.i. e ela precisa fazer uma apresentação desse estudo de caso, portanto não deve prevalecer simplificações e o uso de analogias durante todo o corpo do texto, sem esquecer de se apronfundar na explicação das terminologias próprias da área de cibersegurança. Quero que o formato da explicação demonstre o contexto anterior ao ataque e apresente a cronologia, exemplo: "contexto: '...' cronologia: 01/03/2026 -> explicação do acontecimento"

### Resultado
Para a sua apresentação técnica, este estudo de caso analisa uma campanha de Engenharia Social e Malware que explora a popularidade de ferramentas de Inteligência Artificial para comprometer sistemas através de técnicas avançadas de evasão e persistência.
Contexto do Ataque
O cenário de ameaças em 2026 é marcado por uma quebra de equilíbrio na segurança cibernética devido ao avanço das capacidades ofensivas de modelos de IA, como o Claude Mythos, que demonstrou capacidade autônoma de descobrir e explorar vulnerabilidades em larga escala
. Com o Claude atingindo a marca de 290 milhões de visitas mensais, ele se tornou uma isca de alto valor para agentes maliciosos
. O ataque em questão utiliza o prestígio da marca Anthropic para distribuir o PlugX, um RAT (Remote Access Trojan) — um tipo de malware que concede controle remoto total sobre a máquina infectada — operado historicamente por grupos de espionagem
.
Cronologia e Detalhamento Técnico
Fevereiro de 2026 -> Registro de Técnicas Similares Antes da campanha específica do Claude, técnicas de DLL Sideloading utilizando componentes da empresa G DATA foram documentadas publicamente. Esse método de sideloading consiste em induzir um executável legítimo e assinado a carregar uma biblioteca dinâmica (DLL) maliciosa presente no mesmo diretório, explorando a ordem de busca de arquivos do Windows
.
28/03/2026 - 05/04/2026 -> Preparação da Infraestrutura de Phishing Os atacantes ativam registros MX (Mail Exchanger) no domínio fraudulento, utilizando plataformas de envio em massa como Kingmailer e CampaignLark
. O objetivo é sustentar uma campanha de Phishing, que é a prática de enganar usuários através de comunicações eletrônicas para obter dados sensíveis ou instalar software malicioso
.
10/04/2026 -> Descoberta e Análise da Campanha pelo Malwarebytes A investigação revela o funcionamento detalhado do ataque estruturado em camadas
:
Vetor Inicial e Engenharia Social: O usuário é atraído a um site que utiliza Typosquatting (domínios que imitam nomes de marcas reais com pequenos erros) para baixar uma versão "Pro" inexistente do Claude
.
Implantação via Dropper: O arquivo ZIP contém um instalador MSI que coloca os arquivos no caminho C:\Program Files (x86)\Anthropic\Claude\Cluade\. O erro ortográfico "Cluade" permite que o malware coexista com uma instalação real sem substituí-la
. Um atalho é criado para executar um Dropper em VBScript. Na terminologia de segurança, um dropper é um componente de software projetado para "soltar" e instalar a carga maliciosa real sem ser detectado
.
Mecanismo de Persistência: Para garantir a Persistência (a capacidade do malware de permanecer ativo mesmo após reinicializações), o script copia três arquivos para a pasta Startup (Inicialização) do Windows: NOVUpdate.exe (executável legítimo assinado da G DATA), avk.dll (carregador malicioso) e NOVUpdate.exe.dat (carga criptografada)
.
Execução por Sideloading de DLL: O sistema executa o NOVUpdate.exe. Como este programa é assinado digitalmente, ele muitas vezes ignora alertas de ferramentas de Endpoint Security (segurança de terminais). Ao iniciar, ele carrega a avk.dll infectada, que descriptografa e executa o payload do PlugX contido no arquivo .dat
.
Comunicação C2 (Command and Control): Apenas 22 segundos após a infecção, o malware estabelece uma conexão TCP de saída com o endereço IP 8.217.190.58 na porta 443
. O C2 é a infraestrutura central controlada pelo atacante para enviar comandos aos sistemas comprometidos e receber dados exfiltrados
.
Ações Antiforenses: Após o sucesso da infecção, o VBScript utiliza um arquivo batch (.bat) para auto-deleção, apagando os rastros do script inicial no disco para dificultar a análise por especialistas em resposta a incidentes
.
Este ataque demonstra como a sofisticação não reside apenas no código do malware, mas na combinação de ferramentas legítimas (executáveis assinados) com iscas de alta relevância no mercado de tecnologia atual
.

### Considerações
-Estrutura organizada em contexto e linha do tempo.
-Conceitos técnicos explicados de forma clara ao longo da resposta.
-O contexto inicial facilita a compreensão do cenário do ataque.
-A sequência cronológica torna a evolução do ataque mais fácil de acompanhar.
---

## Prompt 5

### Objetivo
Entender qual é foi a linha de raciocínio na construção da resposta dada.

### Prompt
Justifique a organização desta resposta com base nas informações disponíveis nas fontes. Por que os tópicos foram apresentados nessa ordem

### Resultado
A resposta foi organizada em uma sequência lógica, começando pelo contexto do ataque e avançando para sua execução técnica, com base nas informações das fontes. Primeiro, é apresentado o cenário que tornou o Claude um alvo atrativo para os criminosos. Em seguida, a cronologia mostra as etapas de preparação da infraestrutura e da campanha de phishing. Por fim, o ataque é detalhado seguindo sua ordem de execução: download do arquivo, instalação, persistência, exploração por DLL sideloading, comunicação com o servidor C2 e ações antiforenses. Essa estrutura foi escolhida para facilitar a compreensão da relação de causa e efeito entre as diferentes fases do ataque.

### Considerações
-A resposta manteve os principais fatos e explicações apresentados anteriormente.
-Além de preservar as informações iniciais, aprofundou a justificativa da estrutura adotada e da sequência dos acontecimentos.
-A resposta ampliou a compreensão do ataque ao explicar por que cada etapa foi apresentada naquela ordem.
-O foco deixou de ser apenas descrever o ataque e passou a explicar a lógica utilizada na construção da resposta.
---
