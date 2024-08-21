# Zen of Code

### Dicas e Ensinamentos de algumas batalhas já vencidades  

__1 - Prepare o ambiente__

- debugger
- linter
- formats
- gitignore
- ambiente virtual
- comandos ou scritps para executar ações repetitivas
- README

__2 - Entenda o problema__

- procure sempre entender o problema antes de começar a codar, anote observações e pensamentos sobre o projeto.
- crie diagramas e documentação pra deixar claro o que precisa ser feito (whimsical, excalidraw)
- crie TODO's no codigo para se lembrar o que precisa ser feito ou melhorado ao longo do processo
- todo projeto tem regras funcionais, não funcionais e regras de negocio

__3 - Resolva os problema de um jeito inteligente__
	
- pense em mais de uma forma para resolver o problema
- perca um tempo lendo documentação e testando coisas
- não faça uma solução na qual você não sabe ao certo como funciona

__4 - Erros comuns__
	
- codigos monoliticos, ou arquivos com muitas linhas. Um script com centanas ou milhares de linhas 
são terriveis para de debugar, entender, manter e implementar novas fetuares.

- funções ou classe multi-propósito, divida seu projeto em pequenos pedaços que compoe um todo, uma classe ou função deve ser responvel por resolver apenas um pequeno problema

- hardcode, são trechos de codigos que são incluidos como constantes no codigo, imaginando (ou não) que aquele valor não irá ser alterado. Mesmo que fiquemos tentados a fazer esse tipo de inclusão, é necessario a criação de arquivos de configuração, env ou tabelas para carregar esses valores.  

- complexidade de condicionais, scripts qual envolvem estruturas condicionais (if, else if, else, switch case) gigantes na maioria das vezes podem ser resolvidas de forma mais inteligente, uma das formas pode ser incluir return's para 'negativas' em seu codigo deixando assim uma leitura mais linear do seu codigo.

- codigos com dependencia ao ambiente, codigos que não são preparados para roderem em outro ambiente, muitas vezes isso pode estar ligado ao problema de hardcode então sempre use arquivos de configuração podendo-se criar arquivos para varios ambientes mas sempre sendo de facil troca entre ambientes.

- complexidade de algoritmos (for aninhados) são aqueles que possuem mais de um 'for' para realizar algum tipo de função que em grande quantidade de iterações pode provocar algum bound de recursos. lembre-se o resultado de apenas 2 for é o produto deles  

__5 - Dicas__
	
- organize seu codigo
- organize seu tempo
- organize suas tarefas
- nao tenha medo de ter varios arquivos uma para cada finalidade
- trabalhe utilizando sprints
- escreva testes automatizados
- faça a tipagem do seu codigo
- use helper/docstrings de suas funções
- tenha fetuares flags
- tenha tratativas para os erros
- tenha logs
- tenha trace
- tenha metricas
- tenha backup
- tenha rollback

__6 - Escrevendo o README__
	
- Descreva o objetivo do seu projeto
- Stack
- Defina features implementas e que ainda faltam ser feitas.
- Escreva observações sobre seu projeto.
- Como instalar e configurar seu projeto?
- Quais as dependecias?
- Como rodar?
- Defina quem são os usuarios chaves do seu projeto






