# Prettier tag cloud for wowchemy

**Prettier tag cloud** than original wowchemy tag_cloud block!

Implemented by using [wordcloud2.js](https://github.com/timdream/wordcloud2.js).

Based on the codes from [https://blog.cubieserver.de/2020/adding-a-tag-cloud-to-my-hugo-blog/](https://blog.cubieserver.de/2020/adding-a-tag-cloud-to-my-hugo-blog/).
I revised some part of the codes to use with wowchemy block.

You can see the demo on [EvaNOTE](https://evanote.mew.kr/#tags) (my website published with Wowchemy).

Thank you!

## 🌈 Add the Block to your Site

1. Install the block by referencing it in your `config/_defaults/config.yaml`:
   ```yaml
   module:
     imports:
       - path: github.com/evandde/wowchemy-evablocks
   ```
2. Create an instance of your block in `home/`, for example let's create `home/my-block.md`:
   ```markdown
    ---
    widget: 'github.evandde.tagcloud-wc2'

    # This file represents a page section.
    headless: true

    # Order that this section appears on the page.
    weight: 40

    title: 

    content:
    # Choose the taxonomy from `config.toml` to display (e.g. tags, categories)
    taxonomy: tags
    # Choose how many tags you would like to display (0 = all tags)
    count: 0
    # Choose the cloud size (the more words, the less size is recommended)
    cloudsize: 40
    ---
   ```
