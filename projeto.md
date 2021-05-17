# Unifying Stream
Explicação sobre a regra de engócios do aplicativo


○ Linguagens de desenvolvimento: **Typescript** 
1. Background do time é totalmente back-end, com linguagens fortemente tipadas (Java e C). Angular utiliza typescript.
2. Permite fácil manutenção ao longo do tempo, utilizando padrões de projetos orientados a objetos de forma mais simples e fácil de entender.
3. Apesar da curva de aprendizado para novos colaboradores ser maior, dentro do contexto proposto a escolha parece interessante.


○ IDE ou softwares de edição/compilação de código: **VSCode**
1. Integração com plugins de auto-complete;
2. Snippets de código de forma simples (Por exemplo emmet);
```html
div.row
<div class="row"> </div>
OU
div.row>div.col-md-4
<div class="row"> <div class="col-md-4"> </div> </div>
```
3. Configurações de ESlint automática;


○ Definições de padrão de código CSS (OOCSS, BEM...): **OOCSS**
1. Facilitar a manutenção do código para o time;
2. Compatível com a escolha do pré-processador SCSS;
3. Nomes de classes mais enxutos.
○ Pré-processador de CSS: **SCSS**
1. Tem uma boa compatibilidade com o uso de OOCSS;


○ Framework Visual de CSS: **Material Design**
1. O framework Material Design foi escolhido devido à sua fácil integração com o framework Angular. Apesar de existir o ng-bootstrap, a integração com angularMaterial parece mais simples de manter;
2. Outro motivo para escolha do Material, foi o seu design minimalista. Como o time não tem muita especialidade em front-end, um design minimalista não facilita a poluição da interface interferindo diretamente na capacidade cognitiva do usuário;
3. A aplicação sugerida não necessita de muitas features na interface.


○ Framework JavaScript: **Angular**
1. Por padrão ele é mais completo do que React. Não é encessário instalação de bibliotecas para cada funcionalidade;
2. Similaridades com linguagens já utilizadas pelo time (Com possibilidade de injeção de dependências, por exemplo);
3. Como o Angular utiliza o typescript por padrão, fica mais fácil manter o sistema.


○ Gerenciadores de pacotes e de dependência: **npm**
1. A utilização do npm parece mais adequada por conta do suporte e popularidade. Apesar da maior performance do yarn [(Comparação)](https://www.whitesourcesoftware.com/free-developer-tools/blog/npm-vs-yarn-which-should-you-choose/#:~:text=As%20you%20can%20see%20above,pretty%20fast%20when%20using%20Yarn.), para um time que está iniciando com esta tecnologia, utilizar o gerenciador de pacotes padrão parece a escolha mais correta a se fazer;


○ Estilo Arquitetural (Monorepos, Micro front-ends):**Monorepos**
1. A utilização de micro front-ends pode acarretar em um aumento de complexidade desnecessário (Ao menos para início do projeto);
2. A escolha aqui foi utilizar monorepos pois a interface não possui grande complexidade.


○ Padrão Arquitetural (Single Page Application, Server-side rendering,
Serverless-side rendering): **Server-side Rendering**
1. A escolha aqui foi por SSR;
2. Não foi escolhido o estilo de um simples SPA pois é necessário pensar no funcionamento da aplicação em diversos tipos de dispositivos. Não é possível garantir a performance em todos os tipos de dispositivos que vão utilizar a plataforma. Neste caso, um SSR é uma escolha interessante;
3. O sistema de SEO é muito importante (ainda mais para uma aplicação nova no mercado).
4. Serverless-side rendering não foi escolhido para o projeto inicial por conta de segurança com possíveis crawlers que podem acabar onerando muito o sistema.


○ Ferramentas de testes: **Cypress**
1. Não existe a necessidade de instalaçà ode drivers para cada tipo de navegador;
2. Assim como os outros frameworks de testes, possui uma fácil integração com jenkins, circle CI, etc;
3. Esta ferramenta de teste possui uma melhor performance do que o Selenium em relação à execução dos testes [(Comparação)](https://www.lambdatest.com/blog/cypress-vs-selenium-comparison/)


