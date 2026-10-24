# Requisitos e critérios de qualidade

Este documento detalha o que o portfólio Máquinas Orgânicas deve oferecer e quais qualidades serão avaliadas. A presença de um requisito nesta lista não comprova que ele foi integralmente atendido.

## Escopo atual

O site apresenta o projeto artístico, seus registros fotográficos e informações sobre o próprio desenvolvimento. A implementação atual utiliza HTML e CSS, com fotografias entregues pelo Cloudinary.

## Requisitos funcionais

| ID | Requisito | Situação conhecida |
|---|---|---|
| RF-01 | Apresentar informações sobre o projeto artístico Máquinas Orgânicas. | Presente na página atual. |
| RF-02 | Exibir registros fotográficos das obras. | Galeria com 13 imagens confirmadas. |
| RF-03 | Organizar o conteúdo em seções de navegação. | Seções de apresentação, obras e desenvolvimento. |
| RF-04 | Apresentar informações sobre o desenvolvimento do portfólio. | Seção existente; conteúdo pode evoluir. |

## Requisitos não funcionais

| ID | Critério | O que verificar |
|---|---|---|
| RNF-01 | Usabilidade | Seções compreensíveis, navegação clara e relação evidente entre imagens e legendas. |
| RNF-02 | Acessibilidade | Texto alternativo adequado, semântica, contraste, foco visível e navegação por teclado. |
| RNF-03 | Responsividade | Apresentação em larguras de tela distintas, incluindo dispositivos móveis. |
| RNF-04 | Desempenho | Carregamento da página e das fotografias; comportamento dos recursos externos. |
| RNF-05 | Manutenibilidade | Separação de HTML e CSS, organização dos arquivos e documentação atualizada. |

## Validação

Os critérios devem ser verificados por inspeção e testes concretos. Quando uma verificação for realizada, registrar:

- data e contexto do teste;
- dispositivo, navegador ou largura de tela, quando relevante;
- comportamento esperado;
- resultado observado;
- problema encontrado e ação tomada.

Não afirmar conformidade integral com uma diretriz ou critério sem evidências suficientes. Os critérios de acessibilidade estão detalhados em [`acessibilidade.md`](acessibilidade.md).
