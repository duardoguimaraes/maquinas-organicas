# Máquinas Orgânicas

**Um encontro entre arte, tecnologia e desenvolvimento de software.**

Portfólio digital do projeto artístico *Máquinas Orgânicas*, desenvolvido por `Eduardo Guimarães` como Trabalho de Conclusão de Curso (TCC) do curso de Artes Visuais do Instituto Federal de Pernambuco (IFPE - Campus Olinda). Utiliza a construção de uma página web como oportunidade de aproximar o antes e o agora: a produção artística, a formação em Artes Visuais e os estudos em Análise e Desenvolvimento de Sistemas (ADS), curso no qual está no 3º período.

O projeto parte de uma inquietação artística sobre as relações entre humanidade, tecnologia e máquina, e se desdobra em uma investigação prática sobre como essas relações podem ser apresentadas, organizadas e documentadas por meio do desenvolvimento web. A poesia de um ciclo que se fecha.

**Repositório:** [github.com/duardoguimaraes/maquinas-organicas](https://github.com/duardoguimaraes/maquinas-organicas)

---

## 1. Sobre o projeto artístico

Apesar de *Máquinas Orgânicas* ter tomado forma apenas no contexto do TCC de Artes Visuais, a pesquisa é antiga: explora relações entre tecnologia e humanidade ao mesmo tempo que dialoga com estéticas como o Cyberpunk e a ideia de que a ficção não é mais tão ficção assim. As peças foram construídas a partir de madeira, componentes eletroeletrônicos descartados e outros materiais reaproveitados. Todos coletados pelas ruas do Recife, ou doados após o mal funcionamento. Sim, lixo.

O reaproveitamento de resíduos não funciona apenas como uma escolha material: participa da construção de significado das obras. Componentes que perderam sua função tecnológica original passam a integrar uma nova composição artística.

As peças **Razão** e **Emoção** integram o projeto e investigam, por meio da provocação estética, a ideia do ser humano como uma máquina orgânica. A combinação de materiais, estruturas e componentes tecnológicos cria objetos que estabelecem uma relação entre o funcionamento mecânico, a experiência humana e a dimensão simbólica dos materiais.

O projeto artístico está associado ao **Projeto legolixo**.

## 2. Objetivo do portfólio digital

O site tem como objetivo apresentar a produção artística em um ambiente digital próprio, reunindo informações sobre a pesquisa, as obras e seus registros fotográficos.

Além de funcionar como portfólio, o desenvolvimento do site representa uma oportunidade de aplicar conhecimentos de ADS, um convite à reflexão sobre pertencimentos e segregação na educação, cultura e tecnologia.

O site está em desenvolvimento. As funcionalidades e decisões registradas neste documento serão atualizadas conforme forem implementadas e verificadas.

## 3. Interdisciplinaridade: Artes Visuais e ADS

A principal característica deste projeto é o encontro entre duas áreas que, embora possuam métodos e objetivos próprios, podem compartilhar processos de investigação, construção e experimentação.

### Artes Visuais

A formação artística contribui para a maneira como o projeto é concebido e apresentado. A escolha dos materiais, composição dos objetos, relação entre forma e significado e a construção de uma identidade visual são aspectos que atravessam tanto as obras quanto o portfólio.

### Análise e Desenvolvimento de Sistemas

Os estudos em ADS contribuem para transformar a produção em uma experiência digital. Isso envolve estruturar o conteúdo com HTML, definir sua apresentação com CSS, organizar arquivos, compreender a relação entre os elementos da página e utilizar ferramentas de desenvolvimento e versionamento.

### O que essas áreas têm em comum?

O processo artístico e o desenvolvimento de software podem envolver investigação, elaboração de hipóteses, experimentação, avaliação de resultados e revisão de decisões.

Na produção artística, essas etapas participam da construção de uma obra. No desenvolvimento web, ajudam a definir a estrutura, a aparência e o comportamento de uma interface.

A intenção é explorar como conhecimentos de diferentes áreas podem se complementar em um mesmo projeto.

O portfólio torna essa relação concreta: a produção artística é o conteúdo apresentado, enquanto o desenvolvimento web é o meio pelo qual esse conteúdo ganha uma nova forma de circulação.

## 4. Estética, interface e acessibilidade

A estética deve dar protagonismo às obras sem competir com elas. A organização das seções, tipografia, espaçamentos, fotografias e as legendas precisam trabalhar em conjunto para favorecer a leitura e a navegação.

O CSS utiliza fundo escuro, superfícies azul-acinzentadas, texto claro e destaques em turquesa e laranja. A adequação da paleta continuará sendo avaliada em conjunto com a legibilidade e a galeria.

UI e UX neste projeto estão relacionados à hierarquia visual, organização da galeria e à clareza do conteúdo.

### Acessibilidade e WCAG

As [Web Content Accessibility Guidelines (WCAG)](https://www.w3.org/WAI/standards-guidelines/wcag/), publicadas pelo W3C, serão utilizadas como referência de estudo e avaliação. Seus quatro princípios são:

- **Perceptível:** conteúdo disponível por diferentes formas de percepção, incluindo alternativas textuais para imagens informativas.
- **Operável:** navegação e controles utilizáveis por diferentes formas de interação, incluindo teclado.
- **Compreensível:** textos e organização que favoreçam o entendimento.
- **Robusto:** compatibilidade com navegadores e tecnologias assistivas.

O atributo `alt` é um ponto de partida, mas não comprova conformidade com as WCAG. A avaliação também deverá considerar contraste, foco visível, estrutura semântica e navegação por teclado. O estado das verificações será registrado em [Acessibilidade](docs/acessibilidade.md).

## 5. Arquitetura e tecnologias

### Visão atual

O projeto utiliza uma arquitetura web estática, centrada no navegador. O HTML estrutura o conteúdo, o CSS define a apresentação visual e o Cloudinary hospeda e entrega as fotografias. A versão atual não possui backend próprio, banco de dados ou API implementada.

```text
Usuário
   |
Navegador
   |-- index.html
   |-- css/style.css
   └-- Cloudinary (imagens)
```

### Organização dos arquivos

```text
maquinas-organicas/
├── index.html
├── css/
│   └── style.css
├── docs/
│   ├── diario.md
│   ├── requisitos.md
│   ├── arquitetura.md
│   ├── acessibilidade.md
│   └── decisoes/
│       └── modelo-adr.md
├── README.md
└── .gitignore
```

- `index.html`: conteúdo, navegação, seções e referências às imagens.
- `css/style.css`: cores, tipografia, espaçamentos e layout.
- `docs/`: registros detalhados do processo e documentação técnica complementar.
- `README.md`: apresentação do projeto e síntese do estado atual.

A separação entre HTML e CSS distingue conteúdo e apresentação, facilitando a leitura e a manutenção. As imagens são carregadas por URLs externas e não precisam estar armazenadas no repositório. URLs públicas do Cloudinary permitem acesso às imagens por terceiros.

### Ferramentas utilizadas

| Tecnologia ou ferramenta | Utilização no projeto |
|---|---|
| HTML | Estrutura e conteúdo da página |
| CSS | Estilos, cores, tipografia e layout |
| Visual Studio Code | Edição dos arquivos |
| Live Server | Visualização local durante o desenvolvimento |
| Git | Versionamento do código |
| GitHub | Armazenamento remoto do repositório |
| Cloudinary | Hospedagem e entrega das imagens |

O Visual Studio Code é utilizado para editar os arquivos e o Live Server para visualizar as alterações localmente. O Git acompanha as mudanças no código e o GitHub mantém o repositório remoto, permitindo preservar o histórico de versões e separar alterações locais das publicadas.

### Evolução arquitetural

A arquitetura atual atende ao escopo inicial sem exigir frameworks, backend ou banco de dados. Novas tecnologias deverão responder a necessidades identificadas, evitando complexidade desnecessária.

Entre as possibilidades futuras estão melhorias de responsividade e acessibilidade, avaliação de uma Progressive Web App (PWA), investigação de recursos como manifesto e comportamento offline e estudos de desenvolvimento mobile com React Native. Essas possibilidades ainda não integram a arquitetura implementada.

Detalhes da estrutura e das decisões técnicas estão em [Arquitetura](docs/arquitetura.md).

### Aprendizagem e uso de Inteligência Artificial

A Inteligência Artificial Generativa (LLMs) é utilizada como ferramenta de apoio à implementação do projeto, incluindo a escrita e a revisão de código.

Seu uso também faz parte do processo de aprendizagem, permitindo explorar suas possibilidades e limitações, compreender as soluções propostas e avaliar sua aplicação no desenvolvimento de software.

O objetivo é aprender pela prática, utilizando a ferramenta de forma consciente e mantendo a análise crítica das decisões tomadas.

## 6. Requisitos e critérios de qualidade

O site deve apresentar o projeto artístico, exibir registros fotográficos, organizar o conteúdo em seções e informar sobre o desenvolvimento do portfólio. A documentação distingue esses objetivos das qualidades que ainda precisam ser verificadas.

Os critérios de qualidade incluem:

- **Usabilidade:** clareza da navegação e compreensão do conteúdo.
- **Acessibilidade:** acesso por diferentes formas de interação e tecnologias assistivas.
- **Responsividade:** adaptação a diferentes larguras de tela.
- **Desempenho:** carregamento adequado da página e das imagens.
- **Manutenibilidade:** organização do código e da documentação para facilitar alterações.

A inclusão de um requisito não significa que ele já foi integralmente atendido. Sua avaliação dependerá de verificações e testes documentados. A lista detalhada está em [Requisitos](docs/requisitos.md).

Decisões arquiteturais relevantes poderão ser registradas por meio de ADRs (*Architecture Decision Records*), documentando contexto, alternativas, decisão e consequências. O [modelo C4](https://c4model.com/) poderá ser usado futuramente para representar a arquitetura em diferentes níveis de abstração, conforme a complexidade justificar. Esses recursos serão adotados quando contribuírem para compreender e manter o projeto.

## 7. Estado atual do desenvolvimento

O projeto possui uma página HTML, um arquivo CSS separado, uma galeria com 13 imagens hospedadas no Cloudinary e um repositório GitHub. A navegação está organizada em seções de apresentação do projeto, galeria de obras e informações sobre o desenvolvimento.

O layout da galeria está passando por ajustes visuais. A redução da altura das imagens já foi testada, mas a apresentação dos cartões e das legendas ainda precisa ser revista. A documentação também está sendo estruturada para registrar as decisões e acompanhar a evolução do projeto.

## 8. Diário de desenvolvimento

O histórico completo de dificuldades, descobertas, erros, tentativas e soluções está em [`docs/diario.md`](docs/diario.md). O diário registra acontecimentos reais, sem antecipar soluções ou resultados ainda não verificados.

## 9. Próximos passos

### Em andamento

- [ ] Revisar o layout da galeria, especialmente o tamanho dos cartões e o posicionamento das legendas.
- [ ] Ajustar a relação entre imagens, espaços internos, colunas e proporções.
- [ ] Avaliar o comportamento da página em telas de diferentes tamanhos.
- [ ] Revisar os textos alternativos e as legendas das fotografias.
- [ ] Atualizar a documentação à medida que as decisões forem tomadas e verificadas.
- [ ] Revisar as alterações locais antes de publicá-las no GitHub.

### Possibilidades futuras

- [ ] Consolidar a identidade visual e a hierarquia de informações.
- [ ] Investigar alternativas de publicação e hospedagem.
- [ ] Avaliar uma PWA e seus requisitos, caso façam sentido para o projeto.
- [ ] Estudar React Native e comparar desenvolvimento web responsivo, PWA e aplicações mobile.
- [ ] Documentar decisões de acessibilidade, desempenho e manutenção conforme forem trabalhadas.

React Native e PWA são possibilidades de estudo ou evolução, não tecnologias implementadas pela versão atual.

## 10. Princípios do projeto

- **Coerência artística:** a interface deve respeitar o protagonismo e o significado das obras.
- **Clareza:** conteúdo e navegação devem ser compreensíveis.
- **Simplicidade técnica:** a arquitetura deve corresponder às necessidades reais.
- **Aprendizagem prática:** decisões e dificuldades devem contribuir para a formação em ADS.
- **Interdisciplinaridade:** conhecimentos artísticos e tecnológicos podem dialogar sem perder suas especificidades.
- **Documentação contínua:** os registros devem acompanhar o estado real do desenvolvimento.

## 11. Repositório

O código-fonte e a documentação estão disponíveis em [Máquinas Orgânicas — GitHub](https://github.com/duardoguimaraes/maquinas-organicas).

---

Projeto artístico: `Máquinas Orgânicas - uma história legolixo`.

Documento em evolução, atualizado conforme o desenvolvimento do portfólio.
