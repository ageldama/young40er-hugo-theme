

# Young40er - Hugo theme

[영포티](https://namu.wiki/w/%EC%98%81%ED%8F%AC%ED%8B%B0)를 위한 테마! so sweet!

[A theme written for my own blog](https://ageldama.github.io/)

![frontpage](/README.md.d/top.png)

![pagination](/README.md.d/pagination.png)

![single / top](/README.md.d/single-top.png)

![single / tags](/README.md.d/single-tags.png)

![archive / chrono](/README.md.d/archive-chrono.png)

![archive / categories+tags](/README.md.d/archive-categories+tags.png)





## Credits

Based [Archie - Hugo theme](https://github.com/athul/archie), Thanks [@athul](https://athul.github.io/)!


----

## Config Example

```toml
baseURL = "https://ageldama.github.io/"
languageCode = "ko-kr"
title = "영포티! I'm 쏘스윗!"
theme="young40er"
copyright = "© jhyun"


[pagination]
  pagerSize=5


[taxonomies]
  category = "categories"
  tag = "tags"



[services.googleAnalytics]
id = "G-XXXXXXXXXXX"


[params]
	useCDN=false # don't use CDNs for fonts and icons, instead serve them locally.
	subtitle = "...여동생 같아서..."

useDefaultSass=true

defaultSassPrepend="""
@import "../../../../node_modules/hover.css/scss/hover"
"""

headerHtml = """
  <script src="/js/bundle.js"></script>
  <link rel="stylesheet" type="text/css" href="/css/chroma.css" />
"""

headNavPreHtml = """
  <div class="search-form">
      <span class="search-loading-indicator" style="display: none;">&lt;&lt; 💾 검색 중 (searching) &gt;&gt;</span>

      <input id="search-query" name="search-query"
          type="text"
          class="search-query"
          tabindex="1"
          placeholder="🔎 검색 (search)"/>
  </div>
"""

headNavPostHtml = """
<button class="dark-mode-btn" aria-label="toggle dark-mode">🌓 dark?</button>
<button class="snow-mode-btn" aria-label="toggle dark-mode">☃️ snow?</button>
"""


# Main menu Items

[[menu.main]]
name = "🗂️ Archive"
identifier = "archive"
url = "/archive/"
weight = 1

[[menu.main]]
name = "📨 Contact"
identifier = "about"
url = "/myself/"
weight = 2

```

