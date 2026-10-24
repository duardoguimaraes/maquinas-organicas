# Arquitetura de software — Máquinas Orgânicas

## 1. Visão geral

A versão atual é um site web estático, centrado no navegador. O HTML estrutura o conteúdo, o CSS define a apresentação visual e o Cloudinary hospeda e entrega as fotografias.

A versão atual não possui backend próprio, banco de dados ou API implementada.

```text
Usuário
   |
Navegador
   |-- index.html
   |-- css/style.css
   └-- Cloudinary (imagens)
```

## 2. Organização dos arquivos

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
- `docs/`: documentação complementar.
- `README.md`: apresentação e síntese do estado do projeto.

## 3. Hospedagem das imagens

As fotografias são carregadas por URLs externas do Cloudinary, não armazenadas no repositório. URLs públicas permitem que terceiros acessem as imagens. Essa escolha reduz a necessidade de manter os arquivos fotográficos junto do código, mas cria dependência da disponibilidade do serviço e das URLs utilizadas.

## 4. Desenvolvimento e versionamento

- **Visual Studio Code:** edição dos arquivos.
- **Live Server:** visualização local durante o desenvolvimento.
- **Git:** acompanhamento das mudanças no código.
- **GitHub:** repositório remoto e histórico das versões publicadas.

As alterações locais não se tornam parte da versão remota até serem registradas e enviadas ao GitHub.

## 5. Princípios e limitações atuais

A separação entre HTML e CSS distingue conteúdo e apresentação e facilita leitura e manutenção. A arquitetura simples corresponde ao escopo atual; a adoção de tecnologias adicionais deve responder a necessidades identificadas, sem acrescentar complexidade desnecessária.

## 6. Possíveis evoluções — não implementadas

- Melhorias de responsividade e acessibilidade.
- Avaliação de uma Progressive Web App (PWA).
- Investigação de manifesto, instalação e comportamento offline, se houver necessidade.
- Avaliação de Service Worker apenas se um requisito justificar seu uso.
- Estudos de desenvolvimento mobile com React Native.

Essas possibilidades não fazem parte da arquitetura atualmente implementada.

## 7. Referências de documentação

- [C4 model](https://c4model.com/): representação da arquitetura em diferentes níveis de abstração.
- [arc42](https://docs.arc42.org/): estrutura de documentação arquitetural.
- [Architecture Decision Records](https://adr.github.io/): registro de contexto, alternativas, decisão e consequências.

Essas referências poderão ser adotadas de forma gradual, conforme contribuírem para a compreensão e manutenção do projeto.
