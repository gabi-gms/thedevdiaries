# Roadmap Completo para Formação Fullstack Java/Angular

## Fundamentos da computação

### [REVISÃO] Funcionamento geral de um computador
- [x] Processador, memória RAM, armazenamento e dispositivos de entrada e saída.
- [x] Diferença entre hardware e software.
- [x] Como um programa é carregado e executado.

### [REVISÃO] Sistemas operacionais
- [ ] Função de um sistema operacional.
- [ ] Arquivos, diretórios, usuários, permissões e processos.
- [ ] Diferenças gerais entre Windows, Linux e macOS.

### [REVISÃO] Sistemas numéricos
- [ ] Sistema decimal, binário e hexadecimal.
- [ ] Conversão básica entre representações.
- [ ] Representação de números na memória.

### [REVISÃO] Representação de dados
- [ ] Bits e bytes.
- [ ] Texto e Unicode.
- [ ] Imagens, áudio e arquivos binários.
- [ ] Unidades como KB, MB, GB e TB.

### [REVISÃO] História e evolução da computação
- [ ] Linguagens compiladas e interpretadas.
- [ ] Evolução da internet e da computação pessoal.
- [ ] Surgimento da computação em nuvem.

## Terminal e ambiente de desenvolvimento

### [REVISÃO] Linha de comando
- [ ] Navegação entre diretórios.
- [ ] Criação, movimentação, cópia e remoção de arquivos.
- [ ] Execução de programas.
- [ ] Caminhos absolutos e relativos.

### [REVISÃO] Terminal Linux
- [ ] Comandos como `cd`, `ls`, `pwd`, `mkdir`, `cp`, `mv`, `rm` e `cat`.
- [ ] Pipes e redirecionamento.
- [ ] Variáveis de ambiente.
- [ ] Permissões básicas.

### [REVISÃO] Shell
- [ ] Bash, PowerShell e outros shells.
- [ ] Scripts simples.
- [ ] Alias e configuração do terminal.

### [REVISÃO] Instalação e gerenciamento de ferramentas
- [ ] Variável `PATH`.
- [ ] Interpretadores e runtimes.
- [ ] Gerenciadores de pacotes.
- [ ] Versões de linguagens.
- [ ] SDKMAN para instalar e alternar versões do JDK.
- [ ] JDK 21 ou 25 (LTS), Maven, Node.js, Docker e Docker Compose instalados.
- [ ] PostgreSQL rodando em container.

### [REVISÃO] Editor ou IDE
- [ ] Organização do workspace.
- [ ] Extensões.
- [ ] Busca global.
- [ ] Refatoração básica.
- [ ] Terminal integrado.
- [ ] Depurador.
- [ ] IntelliJ IDEA para Java: workspace, busca global, refatoração, terminal integrado, depurador.
- [ ] VSCode para Angular: extensões, depuração no navegador.

## [REVISÃO] Controle de versão
 
- [ ] Repositório, histórico, commit, estados de arquivo.
- [ ] Fluxo básico: `init`, `add`, `commit`, `log`, `restore`.
- [ ] Remotos: `clone`, `push`, `pull`, `fetch`.
- [ ] Branches: criar, trocar, mesclar, excluir.
- [ ] Resolução de conflitos.
- [ ] Boas mensagens de commit.
- [ ] Pull requests: revisão, comentários, aprovação, integração.
- [ ] `rebase`, `cherry-pick` e `reflog` — entender o propósito antes de usar.
- [ ] Feature branches e trunk-based development em nível conceitual.

## [REVISÃO] Lógica de programação
  
- [ ] Algoritmo como sequência de instruções: entrada, processamento, saída.
- [ ] Decompor problema grande em partes menores.
- [ ] Identificar entradas, regras, exceções e resultados a partir de um requisito.
- [ ] Variáveis, constantes e tipos.
- [ ] Operadores aritméticos, relacionais, lógicos e de atribuição.
- [ ] Condicionais e condições compostas.
- [ ] Repetição: `for`, `while`, controle de laço, condição de parada.
- [ ] Funções: parâmetros, retorno, escopo, responsabilidade única.
- [ ] Rastrear manualmente como os dados mudam durante a execução.
- [ ] Ler mensagem de erro, usar breakpoint, inspecionar variável, isolar a origem de um bug.

## Java: linguagem
 
- [ ] JDK, JRE e JVM: o que cada um faz e por que existe bytecode.
- [ ] Estrutura de projeto Maven: `pom.xml`, dependências, ciclo de vida do build.
- [ ] Tipos primitivos, wrappers, autoboxing e suas armadilhas.
- [ ] `var`, `final`, escopo, passagem de parâmetro por valor de referência.
- [ ] Strings: imutabilidade, `StringBuilder`, `String.format`, text blocks.
- [ ] `switch` como expressão.
- [ ] Arrays.
- [ ] Entrada e saída pelo console.

## Java: orientação a objetos
 
- [ ] Classes, objetos, construtores, `this`.
- [ ] Encapsulamento de verdade — não getter e setter para tudo.
- [ ] Herança, `super`, sobrescrita, `@Override`, classes abstratas.
- [ ] Interfaces, `default methods`, programar para a interface.
- [ ] Polimorfismo: quando ele elimina um `if` gigante.
- [ ] Composição em vez de herança, e por que herança é a exceção.
- [ ] `equals`, `hashCode` e `toString`: o contrato entre eles.
- [ ] `records` para dados imutáveis.
- [ ] `enums` com comportamento.
- [ ] Pacotes e modificadores de acesso.
- [ ] `static`: o que é e por que abusar destrói a testabilidade.

## Java: collections e generics
 
- [ ] `List`, `Set`, `Map` — quando usar cada um.
- [ ] `ArrayList` vs `LinkedList`, `HashMap` vs `TreeMap` e o custo de cada operação.
- [ ] Iteração, `Comparator`, ordenação.
- [ ] `ConcurrentModificationException` e por que ela acontece.
- [ ] Generics: tipos parametrizados e wildcards em nível de leitura.
- [ ] Coleções imutáveis e efeitos colaterais de mutabilidade compartilhada.
- [ ] Cópia rasa e cópia profunda.

## Java: erros e valores ausentes
 
- [ ] Checked vs unchecked.
- [ ] `try`, `catch`, `finally`, try-with-resources.
- [ ] Criar exceções próprias com significado de domínio.
- [ ] `Optional`: uso correto no retorno, uso errado em parâmetro e campo.
- [ ] Nunca engolir exceção em silêncio.

## Java moderno
 
- [ ] Lambdas e interfaces funcionais: `Function`, `Predicate`, `Supplier`, `Consumer`.
- [ ] Streams: `map`, `filter`, `reduce`, `collect`, `groupingBy`.
- [ ] Quando stream ajuda e quando um `for` é mais legível.
- [ ] Pattern matching em `instanceof` e `switch`.
- [ ] Sealed classes em nível conceitual.
- [ ] Virtual threads em nível conceitual.
- [ ] Leitura e escrita de arquivos com `java.nio`.
- [ ] JSON com Jackson.

## Testes automatizados
 
Comece aqui, não no fim. Todo código dos próximos blocos nasce com teste.
 
- [ ] Para que serve teste automatizado.
- [ ] JUnit 5: `@Test`, `@BeforeEach`, `@ParameterizedTest`.
- [ ] AssertJ para asserções legíveis.
- [ ] Estrutura Arrange, Act, Assert.
- [ ] Casos de sucesso, de erro e de limite.
- [ ] Testar comportamento, não implementação.
- [ ] Testes determinísticos e fixtures.
- [ ] Mockito: mocks e stubs sem substituir toda a integração real.
- [ ] Cobertura como indicador, nunca como meta.

> **Marco:** aplicação de console com regras de negócio não triviais, persistência em arquivo, tratamento de erros e no mínimo 20 testes. Necessário conseguir explicar por que cada classe existe.
 
## [REVISÃO] Algoritmos e complexidade
 
> O suficiente para entrevista e para não escrever código lento sem perceber.
 
- [ ] Notação Big O, melhor caso, caso médio e pior caso.
- [ ] Custo de tempo e de memória.
- [ ] Arrays, listas, pilhas e filas.
- [ ] Tabelas hash: função de hash, colisão, por que `HashMap` é O(1).
- [ ] Busca linear e busca binária.
- [ ] Recursão: caso-base, pilha de chamadas, risco de recursão infinita.
- [ ] Ordenação: merge sort conceitualmente, `Collections.sort` na prática.
- [ ] Método de resolução: entender, criar exemplos, mapear casos extremos, implementar, testar, analisar complexidade.

## [REVISÃO] Banco de dados relacional
 
- [ ] Modelagem: entidades, atributos, relacionamentos, cardinalidade.
- [ ] Tabelas, linhas, colunas, chave primária e estrangeira.
- [ ] Restrições: `NOT NULL`, `UNIQUE`, `CHECK`, integridade referencial, `ON DELETE`.
- [ ] `SELECT`, `INSERT`, `UPDATE`, `DELETE`.
- [ ] `INNER JOIN`, `LEFT JOIN` e o que muda no resultado.
- [ ] Agregações: `COUNT`, `SUM`, `AVG`, `GROUP BY`, `HAVING`.
- [ ] Filtros, ordenação e paginação.
- [ ] Normalização até a 3FN, e quando desnormalizar de propósito.
- [ ] Índices: propósito, benefício, custo de escrita.
- [ ] Transações e ACID, níveis de isolamento em nível conceitual.
- [ ] `EXPLAIN` para ler um plano de execução simples.
- [ ] Migrations com Flyway: versionar schema como se versiona código.

## [REVISÃO] Redes e HTTP
 
- [ ] Modelo cliente-servidor, IP, portas, protocolos.
- [ ] DNS e resolução de nomes.
- [ ] TCP e UDP em nível conceitual.
- [ ] HTTP e HTTPS: requisição, resposta, cabeçalhos, corpo.
- [ ] Métodos: `GET`, `POST`, `PUT`, `PATCH`, `DELETE`.
- [ ] Códigos de status: famílias 2xx, 3xx, 4xx, 5xx e os específicos que importam (201, 204, 401, 403, 404, 409, 422).
- [ ] JSON como formato de troca.
- [ ] REST como estilo arquitetural.
- [ ] Cookies, sessões e armazenamento no navegador.
- [ ] CORS: o que é e por que quebra seu frontend.

## Spring Boot: fundamentos
 
- [ ] Inversão de controle e injeção de dependência: o problema que resolvem.
- [ ] Container, beans, `@Component`, `@Service`, `@Repository`, `@Configuration`.
- [ ] Injeção por construtor, e por que nunca por campo.
- [ ] Auto-configuração e starters: o que o Spring Boot faz por baixo.
- [ ] `application.yml`, perfis (`dev`, `test`, `prod`) e variáveis de ambiente.
- [ ] Logs com SLF4J: níveis, o que logar, o que nunca logar.

## Spring Boot: API REST
 
- [ ] `@RestController`, mapeamento de rotas, `@PathVariable`, `@RequestParam`, `@RequestBody`.
- [ ] Status codes corretos em cada operação.
- [ ] DTOs de entrada e saída, e por que a entidade nunca vaza para o controller.
- [ ] Bean Validation: `@NotBlank`, `@Email`, `@Positive`, validação customizada.
- [ ] `@RestControllerAdvice` para tratamento centralizado de erros com resposta padronizada.
- [ ] Paginação e ordenação com `Pageable`.
- [ ] Documentação com springdoc-openapi.

## Spring Boot: persistência
 
- [ ] JPA e Hibernate: entidades, `@Id`, estratégias de geração.
- [ ] Relacionamentos: `@OneToMany`, `@ManyToOne`, `@ManyToMany`, `mappedBy`.
- [ ] Lazy vs eager, problema N+1 e como detectá-lo pelo log de SQL.
- [ ] Spring Data JPA: repositórios, query methods, `@Query`.
- [ ] `@Transactional`: escopo, rollback, armadilhas.
- [ ] Quando abandonar o ORM e escrever SQL direto.

## Arquitetura de aplicação
 
- [ ] Camadas: controller, service, repository, domínio.
- [ ] Onde mora a regra de negócio — e por que não é no controller.
- [ ] Alta coesão, baixo acoplamento, dependências explícitas.
- [ ] KISS, DRY e YAGNI aplicados com julgamento, não como dogma.
- [ ] Nomes claros, funções pequenas, separação de responsabilidades.
- [ ] Comentário que explica decisão, não que narra código.
- [ ] Refatoração em passos pequenos e verificáveis.
- [ ] Formatação automática e linter no projeto.

## Segurança
 
- [ ] Validação de entrada e sanitização de saída.
- [ ] SQL Injection, XSS e CSRF.
- [ ] Hash de senha com BCrypt. Nunca texto puro, nunca MD5 ou SHA1.
- [ ] Spring Security: filtros, autenticação, autorização.
- [ ] Autenticação com JWT: emissão, validação, expiração, refresh.
- [ ] Autorização por papel e princípio do menor privilégio.
- [ ] Gerenciamento de segredos: nada de token ou senha no código, no repositório ou no log.
- [ ] HTTPS.
- [ ] OWASP Top 10.

## Testes de backend
 
- [ ] Teste unitário de service com Mockito.
- [ ] `@WebMvcTest` para a camada web isolada.
- [ ] `@SpringBootTest` para integração.
- [ ] Testcontainers: banco real e descartável dentro do teste.
- [ ] Teste de regra de negócio antes de teste de framework.

> **Marco:** API REST completa com autenticação JWT, CRUD com regras reais, paginação, validação, tratamento global de erro, migrations, documentação OpenAPI e testes de unidade e integração.
 
## [REVISÃO] HTML e acessibilidade
 
- [ ] Estrutura de um documento HTML.
- [ ] HTML semântico: cabeçalhos, navegação, conteúdo principal, seções, artigos, rodapé.
- [ ] Formulários: inputs, labels, tipos de campo, validação, botões.
- [ ] Acessibilidade: navegação por teclado, labels, contraste, texto alternativo, foco, leitores de tela.
- [ ] ARIA apenas quando o HTML semântico não for suficiente.

## [REVISÃO] CSS
 
- [ ] Cascata, especificidade e herança.
- [ ] Box model e seletores.
- [ ] Unidades: `px`, `%`, `rem`, `em`, `vh`, `vw`.
- [ ] Flexbox.
- [ ] CSS Grid.
- [ ] Posicionamento.
- [ ] Design responsivo e media queries.
- [ ] Variáveis CSS e organização de estilos.
- [ ] Transições e animações.
- [ ] Estados de interface: carregando, erro, sucesso, lista vazia, desabilitado.
- [ ] Hierarquia visual, consistência, feedback e prevenção de erro.

## [REVISÃO] JavaScript
 
- [ ] Sintaxe, tipos, `const` e `let`, escopo de bloco, hoisting em nível conceitual.
- [ ] Arrays e objetos, desestruturação, spread.
- [ ] Funções, closures, funções de ordem superior.
- [ ] Igualdade, coerção e valores truthy e falsy.
- [ ] Manipulação do DOM e eventos do navegador.
- [ ] Programação assíncrona: callbacks, `Promise`, `async` e `await`.
- [ ] Event loop, call stack, fila de tarefas e microtasks.
- [ ] `fetch` e tratamento de erro assíncrono.
- [ ] Módulos ES.
- [ ] Armazenamento no navegador.
- [ ] DevTools: Console, Network, Elements, Storage.

## TypeScript
 
- [ ] Tipos primitivos e inferência.
- [ ] Interfaces e type aliases.
- [ ] Union types e narrowing.
- [ ] Tipagem de funções e objetos.
- [ ] Tipos opcionais e tratamento de `null` e `undefined`.
- [ ] Generics básicos.
- [ ] Utility types.
- [ ] Por que evitar `any` — e o que usar no lugar (`unknown`).
- [ ] Configuração do compilador e modo estrito.

## Angular
  
- [ ] Angular CLI: gerar projeto, componente, service, rota.
- [ ] Componentes standalone e bootstrap da aplicação.
- [ ] Template, interpolação e binding de propriedade e evento.
- [ ] Signals: `signal`, `computed`, `effect`, `linkedSignal`, `resource`.
- [ ] Detecção de mudança zoneless e por que o Zone.js saiu.
- [ ] Control flow: `@if`, `@for`, `@switch`, `@defer`.
- [ ] `input()` e `output()` como signals.
- [ ] `inject()` e injeção de dependência, escopo de provider.
- [ ] Services e separação entre estado, dados e apresentação.
- [ ] Ciclo de vida de componente.
- [ ] Pipes e diretivas.
- [ ] `HttpClient` com `provideHttpClient`, interceptors funcionais para token e erro.
- [ ] Roteamento: rotas, parâmetros, rotas filhas, lazy loading, guards funcionais.
- [ ] Formulários: Signal Forms e Reactive Forms (o segundo aparece em todo código existente).
- [ ] RxJS só o necessário: `Observable`, `subscribe`, `pipe`, `map`, `switchMap`, `takeUntilDestroyed`.
- [ ] Consumo de API com estados de carregamento, erro e ausência de dados.
- [ ] Renderização de listas e identificação de elementos.
- [ ] Testes com Vitest.
- [ ] Componentização de verdade: quando quebrar um componente em dois.

## Integração e entrega
 
- [ ] Autenticação ponta a ponta: login, armazenamento do token, refresh, logout, rota protegida.
- [ ] CORS configurado corretamente, sem `*`.
- [ ] Build de produção do Angular.
- [ ] Dockerfile do backend e do frontend, orquestração com Docker Compose.
- [ ] CI no GitHub Actions: build, teste e lint a cada push.
- [ ] Deploy em serviço real, com URL pública acessível.
- [ ] Variáveis de ambiente e segredos no ambiente de deploy.
- [ ] Health check e métricas com Actuator.
- [ ] README profissional: o que é, por que existe, como rodar, decisões técnicas.

> **Marco:** sistema completo no ar, com URL pública, repositório organizado e um comando para subir tudo localmente.
 
## Inteligência Artifical como copilota
 
- [ ] Como um modelo de linguagem funciona: tokens, contexto, probabilidade.
- [ ] Limitações: alucinação, contexto incompleto, conhecimento desatualizado, código que roda mas é inseguro.
- [ ] Estruturar pedido técnico: contexto, objetivo, restrição, formato de saída, critério de aceitação.
- [ ] Verificar código gerado: executar, ler, testar, conferir dependências e segurança.
- [ ] Usar IA para explicar, gerar exercício e revisar solução — não para escrever o projeto no seu lugar.
- [ ] Depurar com IA: fornecer o erro, o comportamento esperado e uma reprodução mínima.
- [ ] Nunca enviar segredo, dado pessoal ou código proprietário.
- [ ] A responsabilidade pelo código continua sendo sua.

## Verificação de Evolução
 
> O ponto de chegada não é ter marcado todos os itens acima. É conseguir fazer isto sem tutorial:
 
- [ ] Receber um requisito vago e transformar em modelo de dados e lista de endpoints.
- [ ] Decidir a estrutura de pastas e camadas de um projeto novo em folha.
- [ ] Escolher entre duas abordagens e justificar a escolha.
- [ ] Ler stack trace e log até a causa raiz, sem chute.
- [ ] Entrar em um código que não é seu e entender o fluxo antes de mudar qualquer coisa.
- [ ] Estimar quanto tempo algo vai levar e errar por pouco.
- [ ] Explicar cada decisão técnica dos seus projetos em três minutos.