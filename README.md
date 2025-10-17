# Zen of Code

Ensinamentos obtidos de algumas batalhas já vencidas e perdidas

### 1. entenda o problema

- Procure sempre entenda o problema antes de começar, anote observações, pensamentos e dúvidas sobre o projeto.
- Crie diagramas pra deixar claro o que precisa ser feito (whimsical, excalidraw, tldraw, mermaid)
- Faça o levantamento de requisitos
    - Funcionais
    - Não funcionais
    - Regras de negocio


### 2. prepare o ambiente

- debugger
- linter
- typing-checker
- formats
- gitignore
- makefile, justifile, procfile
- README


### 3. resolva os problemas de um jeito inteligente
	
- Pense em mais de uma forma para resolver o problema
- Perca um tempo lendo documentação e testando coisas
- Não faça uma solução na qual você não sabe ao certo como funciona
- Se seu código está repetitivo, provavelmente essa não é a melhor solução 
- Crie sua solução imaginando o pior cenário, mas cuidado com [Overengineering](https://en.wikipedia.org/wiki/Overengineering)

### 3.1 como enfrentar um problema?
	
#### 3.1.1 antes de resolver o problema:

- qual foi o problema?
- porque ele aconteceu?
- como ele pode voltar a acontecer?
- reproduza o erro, Exemplo Mínimo Reproduzível [EMR](https://stackoverflow.com/help/minimal-reproducible-example)

#### 3.1.2 como resolver um problema?:
- planeje a sua solução
- o que sua alteração pode impactar
- teste sua solução com base no EMR

#### 3.1.3 relexões:
- tenha sangue frio, um problema precisa ser revolvido com calma
- resolva o problema de traz para frente, comece pelo nível mais baixo da aplicação e venha subindo
- o problema não precisa ser resolvido no mesmo dia, anote e volte amanhã
- gambiarra gera mais gambiarra e stress gera mais stress

### 4. anti-padrões
	
- Códigos monolíticos, ou arquivos com muitas linhas. Um script com centenas ou milhares de linhas 
são terríveis para de debugar, entender, manter e implementar novas features.

- Funções ou classe multipropósito, divida seu projeto em pequenos pedaços que compõe um todo, uma classe ou função deve ser responsável por resolver apenas um pequeno problema

- hardcode, são trechos de códigos que são incluídos como constantes no código, imaginando (ou não) que aquele valor não irá ser alterado. Mesmo que fiquemos tentados a fazer esse tipo de inclusão, é necessário a criação de arquivos de configuração, env ou tabelas para carregar esses valores.  

- Complexidade de condicionais, scripts qual envolvem estruturas condicionais (if, else if, else, switch case) gigantes na maioria das vezes podem ser resolvidas de forma mais inteligente, uma das formas pode ser incluir return's para 'negativas' em seu código deixando assim uma leitura mais linear do seu código.

- Códigos com dependência ao ambiente, códigos que não são preparados para rodarem em outro ambiente, muitas vezes isso pode estar ligado ao problema de hardcode então sempre use arquivos de configuração podendo-se criar arquivos para vários ambientes, mas sempre sendo de fácil troca entre ambientes.

- Complexidade de algoritmos (for aninhados) são aqueles que possuem mais de um 'for' para realizar algum tipo de função que em grande quantidade de iterações pode provocar algum bound de recursos. lembre-se o resultado de apenas 2 for é o produto deles  

### 5. o "mínimo" esperado do seu projeto

- Use alguma arquitetura de software (MVC, MVT, SOLID, MICROSERVICES...)
- Padronize os commits do repositorio (git-flow, git-cliff, conventional-commits)
- Use hooks para validar os commits (pre-commit, prek)
- Tenha uma documentação bem escrita (openapi, mkdocs, docusaurus)
- Tenha um ciclo de releases (towncrier)
- Tenha features flags, para habilitar e desabilitar recursos
- Tenha testes automatizados (pytest, jest, hypothesis, cypress, playwrite)
- Separe seus ambientes (desenvolvimento, homologação, produção)
- Use Infraestrutura como código IaC (Terraform, Kubernetes, Docker-Swarm)
- Use CI/CD (Jenkins, Travis, Actions)
- Faça benchmark do seu projeto
- Use opentelemetry (logs, métricas, traces, profile)

### 6. escrevendo seu README

- Descreva o objetivo do seu projeto
- Descreva a estrutura do seu projeto
- Descreva a Stack do projeto
- Descreva observações sobre seu projeto
- Descreva como instalar/configurar/executar seu projeto
- Descreva quem são os usuários envolvidos no projeto


### 7. manifesto ao debugging
créditos da imagem [@guites](https://github.com/guites)

<img src="./debugging-manifesto.png">

