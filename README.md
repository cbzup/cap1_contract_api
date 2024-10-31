## Apresentação 04/11 

* Spring Boot Framework
* SOLID
* CLEAN CODE


* Spring Boot - Conceitos

    * É um framework do ecosystem spring para criação de aplicação configuráveis com base em arquivos de propriedades, em alguma literaturas podemos encontrar definições como, framework spring baseado em convenções. De acordo com a documentação oficial do Spring Boot (recomendo a leitura) esse framework surge à partir da necessidade de dar mais celeridade ao processo de criação e start de aplicação standalone (originalmente conceituado), mas amplamente utilizado hoje no mercado para construção de serviços e aplicações distribuídas, sendo monolíticas e ou modulares.

* Pontos importantes sobre o Spring Boot que demove conhecer, e aprender.

    * Configurações automáticas - Redução das necessidade de configurações manuais, já que o SB pode automatizar esses configurações por meio das suas dependências encontrados no seu classpath;
    * Servidor interno - Aplicações desenvolvidas com SB não necessitam de servidores externos para serem executados, nesse caso o próprio framework trás essas configurações internas com os servidores Jetty, Tomcar e ou Undertow;
    * Simplificação de dependências - Por meio de suas configurações o SB o mecanismo de gerenciamento de dependências atrás do maven e ou gradle, ambos com essa função de forma isolada. Essas dependências podem ser internas, ou seja, dentro dos starters do framework e ou bibliotecas de terceiros;
    * Monitoramento - Monitoramento das métricas da aplicação com a utilização do actuator;
    * Gerenciamento - Gerenciamento das informações da saúde como das métricas através de ferramentas auxiliares como o grafana, por exemplo;
    * Facilidade de teste - O SB fornece integração nativa para criação de testes unitários e de integração, quando trás também de forna nativa, bibliotecas de testes necessárias para executar esse processo;


* Exemplo básico de uma aplicação web baseada em spring framework: Criaremos uma pequena API de contatos ( o famoso crud)


* SOLID - Esse conceito representa alguns princípios relacionados a construção e ao design de um software, idealizado por Uncle Bob (Robert C. Martin) o implante do SOLID e seus conceitos na construção de um sistema, tentam garantir a fina compreensão do sistema, e características como flexibilidade e manutenção.

    * Single Responsibility Principle
        * Qualquer estrutura, seja ela uma classe e ou serviço independente, terá apenas uma única situação que deles exigem qualquer mudança, ou seja, esses componentes devem possuir apenas uma única responsabilidade para existir;
    * Open Close Principle
        * Entidades de código, como classes, funções e até mesmo módulos (dependendo do tipo de estrutura e design da aplicação) deve está permanentemente aberta para extensões, mas nunca para modificações, nesse caso o entendimento é de que, uma classe por exemplo poderá ser estendida mas nunca modificada;
    * Liskov Substituition Principle
        * Objetos frutos de derivações de podem substituir suas classes primarias (classes mãe e ou principais ) sem modificar o comportamento padrão da aplicação, ou seja, subclasse dever ser substituída por sua superclasse;
    * Interface Segregation Principle
        * Interfaces não podem ser assinados por classes (clientes desses contratos) que não devem possuir execuções desses contratos em seus processos, ou seja, uma classe não pode implementar interfaces que estão fora ou não fazem parte de seu contexto de domínio;
    * Dependency Injection Principle
        * Esse principio diz que modelos, módulos e ou camadas de uma aplicação não devem depender de componentes do mesmo tipo de mais baixo nível, em todos os casos todos devem depender e abstrações e não das suas implementações concretas;

* Clean Code

    * Programação defensiva - Antecipe situações indesejadas, fique atento a fluxos inesperados e garanta a funcionalidade de seu sistema;
    * Funções resumidas - Garanta a simplicidade e a lógica de seus métodos, não os torne cansativos e susceptíveis a entendimento dúbio, avalie a composição de métodos privados em seus métodos públicos.
    * Variáveis - Entenda quando uma variável deve existir e seu tempo de vida no processo de chamada do seu código, variáveis globais precisam de um motivo justo e necessário par existir;
    * Testes unitários - Garanta a segurança, confiabilidade e certeza dos seus testes unitários, eles devem refletir de forma fiel o processamento das informações no que diz respeito a suas entradas, processamento e armazenamento (se esse for o caso); 
    * Comentários de códigos - Se seu código precisa de comentário é um grande sinal de que ele tá complexo, isso não que dizer que vc não deva comentar seus código, mas seja coerente, e claro em situações onde existam possibilidade de riscos;
    * Nomes para componentes, classes e métodos - Use sempre padrões de escrita para esses componentes, Snake Case e ou Camel Case sempre são obrigatórios, nomes de classes e métodos devem fazer sentido e está dentro do contexto em que estão inseridos. 
