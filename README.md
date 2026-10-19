# Blog

Hugo, Markdown, un foglio CSS. Nessun tema esterno, JavaScript o dipendenza npm.

## Avvio

Installa [Hugo](https://gohugo.io/installation/) (versione 0.146 o successiva; basta l’edizione standard), poi:

```sh
hugo server -D
```

Apri http://localhost:1313.

## Scrivere

```sh
hugo new content posts/titolo.md
```

Modifica il file in `content/posts/`. Imposta `draft = false` per pubblicarlo. `hello-world.md` è un articolo iniziale di esempio, da modificare o rimuovere.

## Configurare e pubblicare

In `hugo.toml` cambia `baseURL` con il dominio definitivo, `title` e la descrizione. Modifica `content/about.md` per la pagina personale.

```sh
hugo --minify
```

Pubblica la directory `public/` su un hosting statico. Il feed RSS è `/index.xml`. Il sito include sitemap e pagina 404. Non serve un processo Hugo sul server.
