# Test-Driven Development - TDD

O TDD é uma prática de desenvolvimento de software defendido pelo eXtremme Programming o famoso e já mencionado o XP, o TDD é uma sigla em ingês para **Test-Driven Development** que significa Desenvolvimento Orientado a Teste que foi descoberto em 2003 por Kent Beck o engenheiro de software americano e criador do XP.

Essa prática é uma das mais populares na área de desenvolvimento de software que tem como promissa principal escrever e modificar o teste do seu código antes mesmo do código existir, ou seja, você já precisa saber que tipo de resultado seu código espera, então crie testes para verificar isso. Depois o próprio código seria desenvolvido e esse teste já serveria para testar, a grande vantagem desse tipo de abordagem é que independente das alterações feitas em seu código é preciso que ela passe por um teste para validá-lo:

Imagine uma situação onde temos outros programadores, refatorando e melhorando seu código depois que tudo passar nos testes já escritos, certificando-se de que tudo funcione, TDD é essencialmente baseado em testes de unidade, que nada mais é do que validar a parte mínima de seus testes. O sistema também é conhecido como uma unidade, geralmente uma classe ou um método, podemos dizer que o teste de unidade é uma ferramenta, TDD é uma técnica que significa que os testes de unidade podem ser escritos sem ter que escrever TDD e os testes de unidade são independentes de outros testes, então você pode verificar cada parte ou função individualmente.

## O ciclo de desenvolvimento do TDD
#
O ciclo de desenvolvimento TDD (Test Driven Development) consiste em três etapas principais, também conhecidas como ciclo "red-green-refactor". Repita essas etapas sucessivamente para cada recurso ou unidade de código que está sendo desenvolvido. Vamos percorrer cada etapa (Redação XP Educação, 2022):

### Red

A primeira etapa consiste em **escrever um pequeno teste que falhará**. Isso acontece porque o teste está esperando por uma resposta que ainda não existe, já que o código ainda não foi criado.

### Green

Na segunda etapa, o **código já foi criado** e **passa por novos testes** até serem aprovados. Com os testes concluídos e o código funcionando sem erros, o desenvolvedor pode passar para o próximo ciclo.

Nesse momento é importante o profissional entender bem quais são as necessidades do cliente. Assim, ele consegue desenvolver códigos que, quando agregados ao sistema, atendam às expectativas deles.

### Refactor

Por fim, a **última etapa** do ciclo é a de **refatoração do código**. Aqui, é o momento de [analisar o código](https://www.igti.com.br/desenvolvimento-web) que foi criado apenas para ser aprovado no ciclo Green e deixá-lo o mais simples possível.

Dessa forma, é na fase de refatoração do código que ele passa por uma limpeza onde são excluídas as duplicidades, extraídas as classes, interfaces e métodos do sistema. Após concluir essas três etapas para uma funcionalidade específica, o desenvolvedor pode passar para a próxima funcionalidade e repetir o ciclo. O TDD incentiva a criação de testes antes do código de implementação, o que ajuda a garantir que o código esteja correto, seja testável e siga as especificações desejadas. Além disso, o processo de refatoração contínua ajuda a manter um código saudável ao longo do tempo.
Uma forma de lembrar esse ciclo é: primeiro faça , depois faça certo e depois faça melhor.

Além das etapas do ciclo, os testes realizados a partir da técnica TDD segue o **Modelo FIRST** (Redação XP Educação, 2022):

- **F (Fast/Rápido):** as testagens são ágeis, já que uma unidade é verificada por vez;
- **I (Isolated/Isolado):** cada teste é feito de forma individual, sem nenhuma integração com o sistema;
- **R (Repeatable/Repetível):** as verificações são repetidas diversas vezes, a fim de analisar o comportamento da unidade em teste;
- **S (Self-verifying/Auto verificação):** checagem do teste, se foi aprovado ou se novas falhas foram identificadas;
- **T (Timely/Oportuno):** o teste deve ser oportuno e trazer novas informações para o desenvolvimento do software.

Adotar o TDD vai fazer com que o programador em um curto prazo não vai mais perder tempo depurando e tentando encontrar as falhas e não terá códigos desnecessários pois o código será pensado simplesmente para passar no teste e no fim teremos um código com mais confiabilidade e mais qualidade. Por essas razões para ter uma noção de que essa perda de tempo é realmente mito sem falar no momento que o código for alterado o ganho de tempo será ainda maior já que o teste para aquela funcionalidade já existe então se ganha no curto, médio e no longo prazo. 

Existem várias ferramentas e framework para se utilizar o TDD na sua linguagem favorita assim é possível ganhar mais tempo e qualidade no seu software associando as práticas do TDD.  Abaixo, vou listar alguns frameworks populares e suas respectivas linguagens:

1. **Python:**
    - **unittest**: O módulo de teste padrão da biblioteca Python permite criar testes unitários.
    - **pytest**: Uma estrutura de teste popular com suporte a testes unitários, integração e funcionalidades avançadas.
    - **nose2**: Outra biblioteca popular que aprimora o unittest padrão com recursos adicionais.
2. **Java:**
    - **JUnit**: Uma das estruturas de teste mais conhecidas e amplamente utilizadas para testes unitários em Java.
    - **TestNG**: Uma alternativa ao JUnit, com suporte a testes de integração e recursos adicionais.
    - **Mockito**: Biblioteca para criação de objetos simulados (mocks) para testes de unidade.
3. **JavaScript (Node.js):**
    - **Mocha**: Uma estrutura de teste amplamente usada para JavaScript/Node.js, com suporte a testes assíncronos.
    - **Jest**: Outra estrutura popular para testes de JavaScript, conhecida por sua simplicidade e configuração fácil.
    - **Sinon.js**: Biblioteca para criação de espiões, stubs e mocks em testes.
4. **C# (.NET):**
    - **NUnit**: Estrutura de teste amplamente utilizada para C# e .NET, semelhante ao JUnit.
    - [**xUnit.net](http://xunit.net/):** Uma alternativa moderna ao NUnit com foco em desempenho e recursos adicionais.
5. **Ruby:**
    - **RSpec**: Uma estrutura de teste popular e altamente legível para Ruby.
    - **MiniTest**: Uma estrutura de teste de unidade simples e leve para Ruby.
6. **PHP:**
    - **PHPUnit**: A estrutura de teste padrão para PHP, inspirada no JUnit.
7. **C++:**
    - **Google Test (GTest)**: Estrutura de teste amplamente utilizada para C++ com uma sintaxe próxima à do xUnit.
8. **Go:**
    - **testing**: A biblioteca de teste padrão do Go, que fornece recursos para testes unitários e de benchmarking.

Esses são apenas alguns exemplos de ferramenta ou framework populares em suas respectivas linguagens. Cada um deles é adequado para diferentes tipos de projetos e possui comunidades ativas de desenvolvedores que os suportam e os mantêm atualizados. A escolha da ferramenta ou framework adequado dependerá das necessidades específicas do projeto e das preferências da equipe de desenvolvimento.

Para entender melhor na prática de como funciona o TDD sugiro ver o tutorial do Paulo Gonçalves onde mostra um exemplo da máquina de venda automática https://github.com/PauloGoncalvesBH/aprenda-tdd-na-pratica.

# BDD (Behavior-Driven Development) na prática

BDD (Behavior Driven Development) é uma metodologia de desenvolvimento de software que visa coordenar desenvolvimento, teste e atividades de negócios em um processo colaborativo. Essa prática foi projetada para melhorar a comunicação e o entendimento entre os membros da equipe de desenvolvimento e as partes interessadas do projeto. O BDD se baseia nos princípios do TDD (Test Driven Development), mas se concentra mais na linguagem e no comportamento do software da perspectiva do usuário final. Ele incentiva a criação de testes automatizados com base em cenários específicos de comportamento esperado do sistema, descritos em linguagem natural que tanto desenvolvedores quanto não desenvolvedores podem entender.
Para Gizele, não é apenas a equipe de desenvolvedores que escreve os cenários de testes. Sendo assim, **três agentes interagem para criar o produto**: o Product Owner (PO), o Quality Analyst (QA) e o developer. É o que Georgie Dinwiddie chamou de “regra dos três amigos”. Assim, se obtém melhores resultados na descrição dos testes.

Enfim, busca-se respostas para algumas questões, como:

- o que testar;
- como denominar os testes;
- como entender porque um teste falha;
- onde iniciar.

## Vantagem
#
A principal vantagem do BDD é que ele ajuda a remover a ambigüidade na comunicação entre os membros da equipe e garante que todos tenham um entendimento comum da funcionalidade do sistema. Como os testes são escritos em linguagem natural, os envolvidos no projeto, mesmo sem conhecimento técnico profundo, podem facilmente revisá-los e validá-los.

O BDD é frequentemente usado em conjunto com práticas ágeis de desenvolvimento de software porque complementa uma mentalidade de entrega iterativa e colaborativa. É amplamente utilizado por equipes de desenvolvimento que buscam melhorar a qualidade do software, minimizar erros, retrabalhos e  mantém um processo de desenvolvimento que atenda melhor às necessidades dos usuários finais.

No ponto de vista da Gizele, traz vantagem como: 

- **melhoria da comunicação**: geralmente, cada pessoa da equipe trabalha em uma etapa quando se refere a um software. Contudo, com o BDD, developers e testadores (as) trabalham integrados. Assim, a metodologia gera mais compartilhamento de conhecimento.
- **visão do todo**: com o trabalho realizado de forma integrada, tem-se uma visão de todas as etapas do processo de desenvolvimento e testagem do software.
- **documentação dinâmica**: as equipes podem documentar mais facilmente o sistema, sem gastar um esforço adicional para isso.

Ainda com as ideia da autora falando sobre cenários, portanto, a facilidade trazida pelo BDD na comunicação entre a equipe, veja um modelo de testes do BDD em que cada cenário é dividido em 3 blocos:

- Given: **dado** um determinado contexto (tem-se determinada reação);
- When: **quando** ocorrer algo;
- Then: **então** se espera algo.

Exemplo: **dada** (given) uma nova promoção, **quando** (then) ela for lançada oficialmente, **então** (then) será enviada uma notificação a um determinado grupo.

Paralelamente, uma série de frameworks é utilizada, como: Jbehave, EasyB e Spock.

## Relação entre BDD e TDD:
#
O BDD utiliza a prática do TDD para a implementação dos testes automatizados baseados nos cenários descritos em linguagem natural. Enquanto o TDD se concentra nos testes unitários e na verificação do comportamento interno do código, o BDD usa os testes como uma forma de especificar o comportamento externo do software, de acordo com a perspectiva do usuário. Portanto, o BDD é uma abordagem mais abrangente que incorpora o TDD em um contexto mais amplo de comunicação e colaboração entre a equipe de desenvolvimento e os stakeholders do projeto. O BDD estende o conceito de TDD, colocando ênfase no comportamento do software e fornecendo uma maneira estruturada e clara de expressar requisitos e especificações de forma colaborativa e orientada ao negócio.

## Conclusão

Ambas as práticas encorajam uma abordagem iterativa e colaborativa no desenvolvimento de software, proporcionando maior clareza sobre os requisitos e comportamentos esperados do sistema. Ao adotar essas práticas, as equipes podem obter códigos mais confiáveis, fáceis de manter e com maior aderência aos objetivos do projeto, resultando em um produto final de maior qualidade e satisfação do cliente. O TDD e o BDD são abordagens valiosas que podem ser aplicadas em diferentes contextos de desenvolvimento, proporcionando benefícios significativos em termos de produtividade, eficiência e confiabilidade do software.

## Referência:

**Redação XP Educação, 2022:** [https://blog.xpeducacao.com.br/tdd-test-driven-development/#:~:text=Qual o significado de TDD,a uma de forma isolada](https://blog.xpeducacao.com.br/tdd-test-driven-development/#:~:text=Qual%20o%20significado%20de%20TDD,a%20uma%20de%20forma%20isolada).

**Paulo Gonçalves:** https://github.com/PauloGoncalvesBH/aprenda-tdd-na-pratica.
