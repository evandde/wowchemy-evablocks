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
   
   ---
   
   # Wowchemy에서 사용할 수 있는 더 예쁜 태그클라우드

Wowchemy가 제공하는 tag_cloud block보다 **더 예쁜 태그클라우드**!

[wordcloud2.js](https://github.com/timdream/wordcloud2.js)를 사용하여 제작하였습니다.

[https://blog.cubieserver.de/2020/adding-a-tag-cloud-to-my-hugo-blog/](https://blog.cubieserver.de/2020/adding-a-tag-cloud-to-my-hugo-blog/) 블로그에서 소개하는 코드를 기반으로 제작하였습니다. 이 코드를 wowchemy block으로서 사용할 수 있도록 일부분을 수정한 것입니다.

실제 사용예시를 [EvaNOTE](https://evanote.mew.kr/#tags)에서 확인할 수 있습니다. (Wowchemy로 만든 저의 개인 블로그입니다)

감사합니다!

## 🌈 사이트에 이 블록을 추가하는법

1. `config/_defaults/config.yaml`의 모듈 부분에 다음의 코드를 추가하여 블록 설치:
   ```yaml
   module:
     imports:
       - path: github.com/evandde/wowchemy-evablocks
   ```
2. 블록을 구현하기 위한 md파일을 생성. 예를 들어, `home/my-block.md`와 같은 파일을 만들고 다음의 코드 추가:
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

