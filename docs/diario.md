# Diário de desenvolvimento — Máquinas Orgânicas

Este documento registra a evolução prática do portfólio em ordem cronológica. As entradas devem descrever acontecimentos reais: dificuldades, tentativas, resultados observados, decisões e aprendizados. Não registrar uma hipótese como se fosse solução confirmada.

## Diário 01 — Separando o código das imagens

**O que aconteceu:** o repositório foi reorganizado para manter o código-fonte separado dos arquivos fotográficos.

**A dificuldade:** as imagens precisavam continuar aparecendo no site sem depender de uma pasta de fotografias dentro do repositório público.

**O que foi feito:** utilização do Cloudinary para hospedar as imagens e referenciá-las diretamente no HTML por meio de URLs.

**O que aprendi:** o navegador pode carregar recursos externos sem que esses arquivos estejam armazenados junto do código. Isso ajuda a separar responsabilidades, embora seja necessário considerar a disponibilidade do serviço externo e a natureza pública dos links.

## Diário 02 — Entendendo a galeria

**O que aconteceu:** a página passou a apresentar as 13 imagens em uma galeria organizada em colunas.

**A dificuldade:** as fotografias ocupavam muito espaço na tela, e reduzir apenas a altura das imagens não resolvia o tamanho visual dos cartões que as envolviam.

**O que foi feito:** foram testados ajustes nas regras de altura, nas imagens e nos espaçamentos do CSS.

**O que ficou pendente:** encontrar uma composição mais equilibrada entre tamanho das obras, cartões, legendas e espaço disponível. As tentativas feitas até agora não produziram o resultado visual desejado.

**O que aprendi:** a aparência de um componente depende da interação entre diferentes regras de CSS. Reduzir uma imagem não reduz necessariamente todo o espaço ocupado pelo elemento que a contém.

## Diário 03 — Documentando o processo

**O que aconteceu:** foi iniciada a criação do README para reunir informações sobre o projeto artístico e o desenvolvimento do site.

**A dificuldade:** registrar o trabalho sem confundir funcionalidades existentes com ideias para o futuro.

**O que estou fazendo:** organizando a documentação em arquivos que separam o contexto artístico, as decisões técnicas, a arquitetura, as dificuldades e os próximos passos.

**O que aprendi:** documentar não é apenas descrever o resultado. Também é registrar as razões das escolhas e deixar claro o que ainda precisa ser resolvido.

> O diário será atualizado à medida que novas etapas forem realizadas. Os relatos futuros deverão refletir acontecimentos reais, sem antecipar soluções ou resultados.
