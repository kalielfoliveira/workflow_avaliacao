# Dashboard de Hábitos de Estudo

Este repositório contém o fluxo de trabalho (workflow) e a documentação para o desenvolvimento do **Dashboard de Hábitos de Estudo**, um app voltado para acompanhamento e análise de metas, histórico e insights sobre hábitos de estudo.

## Sobre o Projeto

O objetivo deste projeto é criar um aplicativo que permita aos usuários:

- **Definir e acompanhar metas de estudo**
- **Visualizar o histórico de atividades**
- **Obter insights personalizados sobre seu desempenho**

O app será desenvolvido seguindo práticas modernas de DevOps, garantindo colaboração eficiente, versionamento seguro e entregas contínuas.

## Estrutura do Repositório

| Arquivo         | Descrição                                      |
|-----------------|------------------------------------------------|
| `WORKFLOW.md`   | Detalhamento completo do fluxo de trabalho     |
| `README.md`     | Visão geral e instruções iniciais              |

## Seções do App

- **Metas:** Cadastro e acompanhamento de metas de estudo semanais/mensais.
- **Histórico:** Registro e visualização das atividades realizadas.
- **Insights:** Análises e gráficos para ajudar na evolução dos estudos.

## Documentação do Workflow

O desenvolvimento do app seguirá um workflow baseado em GitHub Flow adaptado, com branches específicas para features, correções e releases. Para detalhes completos sobre branches, convenções de commits e políticas de integração, consulte:

- [WORKFLOW.md](./WORKFLOW.md)

## Tecnologias & Práticas

- Git & GitHub Flow (variação adaptada)
- Pull Requests obrigatórios
- Commits semânticos
- Integração contínua

## Como Contribuir

1. Crie uma branch a partir de `dev`
2. Siga as convenções de nomeação e commits
3. Abra um Pull Request para revisão
---

## Resolução de Conflitos

Às vezes, duas pessoas mudam o mesmo arquivo (ou até a mesma linha) em branches diferentes. Quando isso acontece e tentamos juntar (merge) essas branches, o Git pode mostrar um **conflito**.

### Como saber que deu conflito

Se você tentar fazer um merge (por exemplo, `git merge dev` na `main`) e o Git avisar que há conflito, ele vai mostrar o(s) arquivo(s) com problema.

### Como resolver

1. Abra o arquivo e veja onde está o conflito.
2. Escolha qual parte do texto faz sentido manter (ou junte as duas).
3. Apague os marcadores (`<<<<<<<`, `=======`, `>>>>>>>`).
4. Salve o arquivo.
5. Adicione ao stage:  
   `git add nome-do-arquivo`
6. Finalize o merge com um commit, se precisar:  
   `git commit`

Depois disso, siga normalmente com os testes e o Pull Request.

**Dicas:**  
- Avise o time se o conflito for complicado.
- Resolva junto se for algo importante.
- Sempre teste depois de resolver.

---

* Commits pequenos e frequentes facilitam a revisão.
* Nunca use `push --force` na branch `main`.
* Sempre crie uma branch nova a partir da `dev` para