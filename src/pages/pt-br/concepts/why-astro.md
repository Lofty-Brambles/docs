---
layout: ~/layouts/MainLayout.astro
title: Por que Astro?
description: "Astro é um framework web tudo em um para construção de websites rápidos, centrados em conteúdo. Aprenda mais."
i18nReady: true
---

Astro é um **framework web** **tudo em um** para a construção de **websites rápidos**, **focados em conteúdo**.

Por que escolher Astro ao invés de outro framework web? Aqui estão cinco princípios de design para te ajudar a explicar o porquê criamos Astro, os problemas que ele resolve e porquê Astro pode ser a melhor escolha para o seu projeto ou time.

#### Astro é...

1. [Focado em conteúdo](#focado-em-conteúdo): Astro foi feito para websites ricos em conteúdo.
2. [Servidor em primeiro lugar](#servidor-em-primeiro-lugar): Websites são mais rápidos quando eles renderizam HTML no servidor.
3. [Rápido por padrão](#rápido-por-padrão): Deve ser impossível construir um website lento com Astro.
4. [Fácil de utilizar](#fácil-de-utilizar): Você não precisa ser um especialista para construir algo com Astro.
5. [Cheio de funcionalidades, porém flexível](#cheio-de-funcionalidades-porém-flexível): Mais de 100 integrações Astro para escolher.

## Focado em conteúdo

**Astro foi feito para websites ricos em conteúdo.** Isto inclui a maioria dos sites de marketing, sites de publicação, sites de documentação, blogs, portfólios e alguns sites ecommerce.

Em contraste, a maioria dos frameworks web modernos foram feitos para construir *aplicações web*. Esses frameworks funcionam melhor para construir experiências mais complexas, como aplicações no navegador: painel de navegação de administrador logado, caixas de entrada, redes sociais, listas de afazeres e até aplicações que parecem nativas como [Figma](https://figma.com/) e [Ping](https://ping.gg/).

Esta é uma das mais importantes diferenças para se entender sobre o Astro. O foco em conteúdo do Astro o permite fazer tradeoffs e entregar funcionalidades com performance sem igual que não fariam sentido para frameworks focados em aplicações implementarem.

:::tip
Se o seu projeto cai no segundo campo de "aplicações", Astro pode não ser a escolha certa para seu projeto... **e tá tudo certo!** Veja o [Next.js](https://nextjs.org/) como alternativa para um ótimo framework web focado em aplicações.
:::

## Servidor em primeiro lugar

**Astro aproveita ao máximo renderização no lado do servidor no lugar de renderização no lado do cliente sempre que possível.** Esta é a mesma abordagem que frameworks no lado do servidor tradicionais -- PHP, WordPress, Laravel, Ruby on Rails, etc. -- vem utilizando por décadas. Porém você não precisa aprender uma segunda linguagem no lado do servidor para utilizá-lo. Com Astro, tudo ainda é apenas HTML, CSS e JavaScript (ou TypeScript, se preferir).

Esta abordagem se destaca em contraste com outros frameworks web JavaScript como Next.js, SvelteKit, Nuxt, Remix e outros. Esses frameworks precisam de renderização no lado do cliente para o seu website inteiro e possuem renderização no lado do servidor principalmente para lidar com problemas de performance. Essa abordagem foi apelidada de **Aplicação de Página Única (SPA, do inglês, "Single Page Application")**, em contraste com a abordagem de **Aplicação de Múltiplas Páginas (MPA, do inglês, "Multi Page App")** do Astro.

O modelo SPA tem seus benefícios. Porém, eles vem com o custo de complexidade adicional e tradeoffs de performance. Esses tradeoffs prejudicam a performance da página -- incluindo métricas críticas como [Time to Interactive (TTI)](https://web.dev/interactive/) -- que não fazem muito sentido para websites focados em conteúdo onde a performance do primeiro carregamento é essencial.

📚 [Aprenda mais sobre o que faz a arquitetura MPA do Astro única.](/pt-br/concepts/mpa-vs-spa/)


## Rápido por padrão

Boa performance é sempre importante, mas é *especialmente* crítica para websites focados em conteúdo. Já foi bem provado de que uma performance ruim te faz perder engajamento, conversões e dinheiro. Por exemplo:

- Cada 100ms mais rápido → 1% mais conversões ([Mobify](https://web.dev/why-speed-matters/), ganhando +$380.000/ano)
- 50% mais rápido → 12% mais vendas ([AutoAnything](https://www.digitalcommerce360.com/2010/08/19/web-accelerator-revs-conversion-and-sales-autoanything/))
- 20% mais rápido → 10% mais conversões ([Furniture Village](https://www.thinkwithgoogle.com/intl/en-gb/marketing-strategies/app-and-mobile/furniture-village-and-greenlight-slash-page-load-times-boosting-user-experience/))
- 40% mais rápido → 15% mais registros ([Pinterest](https://medium.com/pinterest-engineering/driving-user-growth-with-performance-improvements-cfc50dafadd7))
- 850ms mais rápido → 7% mais conversões ([COOK](https://web.dev/why-speed-matters/))
- Cada 1 segundo mais lento → 10% menos usuários ([BBC](https://www.creativebloq.com/features/how-the-bbc-builds-websites-that-scale))

Em vários frameworks web, é fácil construir um website que parece ótimo durante o desenvolvimento para então carregar de forma dolorosamente lenta após o deploy. JavaScript é geralmente o culpado, já que os celulares de usuários e dispositivos menos potentes raramente se comparam a velocidade do notebook de um desenvolvedor.

A mágica do Astro é em como ele combina os dois valores explicados acima -- um foco em conteúdo com uma arquitetura MPA com o servidor em primeiro lugar -- para fazer tradeoffs e entregar funcionalidades que outros frameworks não conseguem. O resultado é uma incrível performance web para todos os sites, fora da caixa. Nosso objetivo: **Deve ser praticamente impossível construir um website lento com Astro.**

Um website Astro pode [carregar 40% mais rápido com 90% menos JavaScript](https://twitter.com/t3dotgg/status/1437195415439360003) do que um mesmo site feito com o mais popular framework web React. Mas não tome nossa palavra sobre isso: veja a performance do Astro deixar Ryan Carniato (criador do Solid.js e Marko) [sem palavras](https://youtu.be/2ZEMb_H-LYE?t=8163).

## Fácil de utilizar

**O objetivo do Astro é de ser acessível para todos os desenvolvedores web.** Astro foi feito para parecer familiar e acessível independente do nível de habilidade ou experiência com desenvolvimento web.

Nós começamos nos certificando de que você poderia usar qualquer uma das suas linguagens de componentes de UI conhecida. React, Preact, Svelte, Vue, Solid, Lit e vários outros são suportados para criar componentes UI novos em um projeto Astro.

Nós também queríamos ter certeza de que Astro teria uma ótima linguagem de componentes integrada também. Para fazer isso, nós criamos nossa própria linguagem de UI `.astro`. Ela é altamente influenciada pelo HTML: qualquer pedaço de código HTML já é um componente Astro válido! Mas ela também combina alguma das nossas funcionalidades favoritas emprestadas de outras linguagens de componentes como expressões JSX (React) e escopeamento do CSS por padrão (Svelte e Vue).

Astro foi feito para ser menos complexo do que outros frameworks e linguagens de UI. Um grande motivo para isso é que Astro foi feito para ser renderizado no servidor, não no navegador. Isso significa que você não precisa se preocupar sobre: hooks (React), stale closures (também do React), refs (Vue), observables (Svelte), atoms, selectors, reactions ou derivations. Também não há reatividade no servidor, então toda essa complexidade não existe.

Um dos nossos provérbios favoritos é: **opte por mais complexidade.** Nós fizemos Astro para remover toda "complexidade obrigatória" que fosse possível da experiência do desenvolvedor, especialmente quando você está iniciando. Você pode construir um website "Olá Mundo" de exemplo com Astro com apenas HTML e CSS. Então, quando você precisar construir algo mais potente, você pode incrementalmente  utilizar funcionalidades e APIs novas na hora. 


## Cheio de funcionalidades, porém flexível

**Astro é um framework web tudo em um que vem com tudo o que você precisa para construir um website.** Astro inclui uma sintaxe de componentes, roteamento baseado em arquivos, manipulação de assetes, processo de build, bundling, otimizações, busca de dados e mais. Você pode construir ótimos websites sem se aproximar de funcionalidades fora do núcleo do Astro.

Se você precisar de mais controle, você pode expandir o Astro com [+100 integrações](https://astro.build/integrations/) como [React](https://www.npmjs.com/package/@astrojs/react), [Svelte](https://www.npmjs.com/package/@astrojs/svelte), [Vue](https://www.npmjs.com/package/@astrojs/vue), [Tailwind CSS](https://www.npmjs.com/package/@astrojs/tailwind), [MDX](https://www.npmjs.com/package/@astrojs/mdx),[otimização de imagens](https://www.npmjs.com/package/@astrojs/image) e mais. [Conectar o seu CMS favorito](https://astro.build/integrations/) ou [fazer deploy para seu host favorito](/pt-br/guides/deploy/) com apenas um comando.

Astro é agnóstico a UI, o que significa que você pode **Trazer o seu Próprio Framework de UI (BYOF, do inglês, "Bring Your Own Ui Framework")**. React, Preact, Solid, Svelte, Vue e Lit são todos oficialmente suportados no Astro. Você pode até misturar diferentes frameworks na mesma página, fazendo migrações futuras mais fáceis e prevenindo que você fique preso a um único framework.
