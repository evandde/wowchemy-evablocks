# Prettier tag cloud for wowchemy

**Prettier tag cloud** than original wowchemy tag_cloud block!

Implemented by using [wordcloud2.js](https://github.com/timdream/wordcloud2.js).

Based on the codes from [https://blog.cubieserver.de/2020/adding-a-tag-cloud-to-my-hugo-blog/](https://blog.cubieserver.de/2020/adding-a-tag-cloud-to-my-hugo-blog/).
I revised some part of the codes to use with wowchemy block.

You can see the demo on [EvaNOTE](https://evanote.mew.kr/#tags) (my website published with Wowchemy).

Thank you!

## ๐ Add the Block to your Site

1. Add the [wordcloud2.js](https://raw.githubusercontent.com/timdream/wordcloud2.js/gh-pages/src/wordcloud2.js) file to your `static/js/` directory.

2. Install the block by referencing it in your `config/_defaults/config.yaml`:
   ```yaml
   module:
     imports:
       - path: github.com/evandde/wowchemy-evablocks
   ```
3. Create an instance of your block in `home/`, for example let's create `home/my-block.md`:
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
   
3. Add the [wordcloud2.js](https://raw.githubusercontent.com/timdream/wordcloud2.js/gh-pages/src/wordcloud2.js) file to your `static/js/` directory.

 ---
   
 # Wowchemy์์ ์ฌ์ฉํ  ์ ์๋ ๋ ์์ ํ๊ทธํด๋ผ์ฐ๋

Wowchemy๊ฐ ์ ๊ณตํ๋ tag_cloud block๋ณด๋ค **๋ ์์ ํ๊ทธํด๋ผ์ฐ๋**!

[wordcloud2.js](https://github.com/timdream/wordcloud2.js)๋ฅผ ์ฌ์ฉํ์ฌ ์ ์ํ์์ต๋๋ค.

[https://blog.cubieserver.de/2020/adding-a-tag-cloud-to-my-hugo-blog/](https://blog.cubieserver.de/2020/adding-a-tag-cloud-to-my-hugo-blog/) ๋ธ๋ก๊ทธ์์ ์๊ฐํ๋ ์ฝ๋๋ฅผ ๊ธฐ๋ฐ์ผ๋ก ์ ์ํ์์ต๋๋ค. ์ด ์ฝ๋๋ฅผ wowchemy block์ผ๋ก์ ์ฌ์ฉํ  ์ ์๋๋ก ์ผ๋ถ๋ถ์ ์์ ํ ๊ฒ์๋๋ค.

์ค์  ์ฌ์ฉ์์๋ฅผ [EvaNOTE](https://evanote.mew.kr/#tags)์์ ํ์ธํ  ์ ์์ต๋๋ค. (Wowchemy๋ก ๋ง๋  ์ ์ ๊ฐ์ธ ๋ธ๋ก๊ทธ์๋๋ค)

๊ฐ์ฌํฉ๋๋ค!

## ๐ ์ฌ์ดํธ์ ์ด ๋ธ๋ก์ ์ถ๊ฐํ๋๋ฒ

1. [wordcloud2.js](https://raw.githubusercontent.com/timdream/wordcloud2.js/gh-pages/src/wordcloud2.js) ํ์ผ์ `static/js/` ํด๋์ ์ถ๊ฐ.

2. `config/_defaults/config.yaml`์ ๋ชจ๋ ๋ถ๋ถ์ ๋ค์์ ์ฝ๋๋ฅผ ์ถ๊ฐํ์ฌ ๋ธ๋ก ์ค์น:
   ```yaml
   module:
     imports:
       - path: github.com/evandde/wowchemy-evablocks
   ```
3. ๋ธ๋ก์ ๊ตฌํํ๊ธฐ ์ํ mdํ์ผ์ ์์ฑ. ์๋ฅผ ๋ค์ด, `home/my-block.md`์ ๊ฐ์ ํ์ผ์ ๋ง๋ค๊ณ  ๋ค์์ ์ฝ๋ ์ถ๊ฐ:
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

