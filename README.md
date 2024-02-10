[![Python 3.9](https://shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-3916/)
[![Platform](https://img.shields.io/badge/platform-linux%20%7C%20windows%20%7C%20macos-lightgrey)](Platform)
[![License](https://img.shields.io/github/license/jiahaoli57/FinOL)](License)
[![Document](https://img.shields.io/badge/docs-latest-red)](https://finol.readthedocs.io/en/latest/)

[![](https://dcbadge.vercel.app/api/server/3tEwzBBT)](https://discord.gg/3tEwzBBT)

[//]: # ([![GitHub stars]&#40;https://img.shields.io/github/stars/ai4finol/finol?color=orange&#41;]&#40;https://github.com/ai4finol/finol/stargazers&#41;)


``FinOL`` represents a pioneering open database for facilitating data-driven financial research. As an
ambitious project, it collects and organizes extensive assets from global markets over half a century,
it provides a long-awaited unified platform to advance data-driven OLPS research.

## Echarts

{% raw %}
<div id="main" style="width: 900px;height:400px;"></div>

<script type="text/javascript">
  // 在这里编写你的 ECharts 图表代码
  // 例如：
  var chartDom = document.getElementById('main');
  var myChart = echarts.init(chartDom);
  var option;

  option = {
    title: {
      text: 'Line'
    },
    tooltip: {
      trigger: 'axis'
    },
    legend: {
      data: ['Market', 'Best']
    },
    grid: {
      left: '3%',
      right: '4%',
      bottom: '3%',
      containLabel: true
    },
    toolbox: {
      feature: {
        saveAsImage: {}
      }
    },
    xAxis: {
      // type: 'category',
      // boundaryGap: false,
      // data: ['Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun']
      type: 'value'
    },
    yAxis: {
      type: 'value'
    },
    series: [
      {
        name: 'Market',
        type: 'line',
        data: [0.994430184,1.005787181,1.00641905,1.002685923,1.004306982,0.99984743,1.011696695,1.004420013,0.996788986,0.995406856,0.996675943,0.997097135,1.007216795,0.994210316,0.998043224,1.001463189,0.996676559,0.985535335,0.972887139,0.974191882,0.979657553,0.98688977,0.997617124,0.99501837,0.991825242,1.002323427,0.997483934,0.995766348,0.993911233,0.990437831,1.008304682,1.013423368,1.005717354,0.998870208,0.992953391,0.988174705,0.982568327,0.9841496,0.987376363,0.993866938,0.991994983,0.989781959,0.983463353,0.969491635,0.962016007,0.950669101,0.944767855,0.93941377,0.927291753,0.931230026,0.930489248,0.937737398,0.928014443,0.912116157,0.922650835,0.902570885,0.896367505,0.90153909,0.893162842,0.903112134,0.903996125,0.897208348,0.886753227,0.878888461,0.876760496,0.87942999,0.910070368,0.9119009,0.893997718,0.891515956,0.896791758,0.9014845,0.898275209,0.891328483,0.882973575,0.883590601,0.876696924,0.891185935,0.903146381,0.907525053,0.912517269,0.927865006,0.916970462,0.920352994,0.911593378,0.900052473,0.89626331,0.891072133,0.899507493,0.921057758,0.915144222,0.915082257,0.902910135,0.90105235,0.893230046,0.872882584,0.879185655,0.881620114,0.883255008,0.878217724,0.902098217,0.899209626,0.908083693,0.909719056,0.901224188,0.903206996,0.891840204,0.89887596,0.89940541,0.90909401,0.903345068,0.90817322,0.919074623,0.915753901,0.909859463,0.89187911,0.898223241,0.910539829,0.902907501,0.900240091,0.890745865,0.890847697,0.895598859,0.898471977,0.890007909,0.883053024,0.875570882,0.870912573,0.866871709,0.859407831,0.860135529,0.850759829,0.858043299,0.867586958,0.881050749,0.884367789,0.881816244,0.888852707,0.888563597,0.889687567,0.875112618,0.874245184,0.876796653,0.871512423,0.865572533,0.884289543,0.888228605,0.898504542,0.897755468,0.897058121,0.891178421,0.88714238,0.882167372,0.887155547,0.890021778,0.889209803,0.892879807,0.888106099,0.879762657,0.889965402,0.880757241,0.871179647,0.863825941,0.865814512,0.872847248,0.877072676,0.86777709,0.857735016,0.856110008,0.854827059,0.85101939,0.857265225,0.869798294,0.878181057,0.8697576,0.877248191,0.891415434,0.917020198,0.946000659,0.951045292,0.958426242,0.944767145,0.966836355,0.962620007,0.964078062,0.955124095,0.946341359,0.949051796,0.952379346,0.950902345,0.967485932,0.952986459,0.9603593,0.960966521,0.953280836,0.959118292,0.95410924,0.947120908,0.948845992,0.941864539,0.937917259,0.94330296,0.93123292,0.924372624,0.925434782,0.92452861,0.950356445,0.957392968,0.95667412,0.943333201,0.934878678,0.933877222,0.918566331,0.919866006,0.925485466,0.929929747,0.933935095,0.922956475,0.917572843,0.908646571,0.904964155,0.911473534,0.901986552,0.896573842,0.894751432,0.903287113,0.905338206,0.910191365,0.924188069,0.920632605,0.925793832,0.955862955,0.96333428,0.955574191,0.958156833,0.959240221,0.949281107,0.946037229,0.943864366,0.961048811,0.953109505,0.963383663,0.968196672,0.972004313,0.986265368,0.972108701,0.962877524,0.950521434,0.952206369,0.942364778,0.946705319,0.944907296,0.929250208,0.928029797,0.937225123,0.944970077,0.959609405,0.955965373,0.962970833,0.947744644,0.939110151,0.933983258,0.930270031,0.933931955,0.923860683,0.923182486,0.917911384,0.927252545,0.932532682,0.932536795,0.925579683,0.932788376,0.936428189,0.962782133,0.962358277,0.954068233,0.948611001,0.956057306,0.952287662,0.948859368,0.950613748,0.951988797,0.94247028]
      },
      {
        name: 'Best',
        type: 'line',
        data: [0.99546432,1.0000001,1.0022676,1.0022676,0.98412645,0.97052103,0.98866212,1.0022676,1.0113373,1.0249426,1.0204078,1.015873,1.0181403,1.0181403,1.0294783,1.0408163,1.0340132,1.0249426,1.0068023,0.988662,0.97052085,0.98412627,0.988662,0.988662,1.0022675,0.9931969,0.988662,0.97959143,0.97052085,0.96598601,0.99546432,1.0022675,0.99092948,0.97732401,0.97052085,0.96825337,0.92743707,0.93424022,0.9319728,0.95238048,0.94104248,0.94784558,0.94330984,0.9342401,0.9342401,0.92743695,0.94104236,0.93650752,0.92290205,0.92063463,0.90929663,0.90702921,0.92516959,0.91156411,0.92290211,0.91609895,0.89795864,0.90702921,0.90929663,0.91156405,0.90702915,0.91156399,0.90702909,0.90702909,0.90249342,0.91836715,0.9523803,0.94557798,0.93423998,0.94104224,0.95918339,0.97278881,0.97505629,0.97278887,0.96145087,0.9569152,0.94330972,0.95918345,0.9682532,0.97052062,0.97732371,0.99319661,0.99092919,0.99999976,0.99546409,0.99092925,0.98639435,0.98866177,0.99319655,0.9999997,0.99546403,0.99546403,0.99546403,0.99773145,0.99773145,0.97959113,0.98866171,0.97959113,0.97052056,0.97278887,0.99092913,0.99319661,0.99773151,0.99773151,0.97959119,0.99319655,0.97505629,0.98185861,0.98412603,0.99319661,0.98866171,0.99319649,1.029478,1.0249423,1.0249423,1.0226749,1.0272107,1.0476185,1.0385479,1.022675,1.011337,1.0090696,1.0181402,1.0272108,1.0249425,1.0204077,1.0136054,1.0090697,1.0113372,0.99773169,1.0022674,0.98639452,0.99092942,0.99773169,1.0113372,1.0045348,1.0068023,1.027211,1.0340133,1.0317458,1.0068023,1.0158728,1.0317457,1.0294782,1.0294782,1.0453511,1.0544217,1.0680271,1.0748293,1.0816325,1.0748293,1.0476184,1.0317456,1.0476184,1.0453509,1.0385478,1.0453509,1.0453509,1.0430834,1.0589564,1.0657587,1.0521532,1.0498857,1.0634912,1.0816324,1.0770967,1.0657587,1.0657587,1.056689,1.0476184,1.0476184,1.0544215,1.0634913,1.0929697,1.072562,1.0793642,1.0907022,1.1043077,1.1405891,1.1496598,1.1519272,1.1337861,1.1473914,1.1292511,1.1201805,1.1020402,1.1020402,1.1043075,1.1043075,1.1020401,1.1269835,1.1111107,1.1043075,1.106575,1.106575,1.113378,1.1156455,1.117913,1.1224487,1.1224487,1.113378,1.1315184,1.1201804,1.0975052,1.0952377,1.1020401,1.1292509,1.136054,1.1405889,1.136054,1.1224486,1.1179129,1.1065749,1.1156454,1.1269834,1.1360539,1.1405888,1.1360539,1.1383214,1.1292509,1.1269834,1.1247159,1.1247159,1.1156454,1.0975051,1.1065748,1.1020399,1.1088431,1.1337856,1.147391,1.1428561,1.1746019,1.1700671,1.1723346,1.174602,1.174602,1.18594,1.1768703,1.18594,1.1927432,1.1791377,1.1927432,1.1882075,1.1791377,1.1836725,1.1723346,1.1700671,1.1632648,1.1632648,1.1519268,1.1541942,1.1496594,1.1337857,1.1337857,1.1519269,1.1496594,1.1587291,1.1564616,1.1428561,1.1337855,1.1269832,1.1224483,1.1179127,1.1247157,1.1133777,1.1111103,1.0929692,1.1043072,1.1043072,1.1043072,1.1065747,1.1247157,1.1337855,1.1587288,1.1519265,1.149659,1.1292505,1.1337854,1.1247156,1.1224481,1.1315179,1.1315179,1.1224481]
      }
    ]
  };

  option && myChart.setOption(option);
</script>
{% endraw %}

## How to Get Started

This theme can be used just as other [Jekyll themes][1] and support [remote theme][12],
see [the official guide][13] as well.

You can introduce this jekyll theme into your own site by either

- [Fork][3] this repository and add your markdown posts to the `_posts` folder.
- Use as a remote theme in your [`_config.yml`][14](just like what we do for this
  site itself),

```yaml
remote_theme: sighingnow/jekyll-gitbook
```

### Deploy Locally with Jekyll Serve

This theme can be ran locally using Ruby and Gemfiles.

[Testing your GitHub Pages site locally with Jekyll](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/testing-your-github-pages-site-locally-with-jekyll) - GitHub

## Full-text search

The search functionality in jekyll-gitbook theme is powered by the [gitbook-plugin-search-pro][5] plugin and is enabled by default.

[https://sighingnow.github.io/jekyll-gitbook/?q=generated](https://sighingnow.github.io/jekyll-gitbook/?q=generated)

## Code highlight

The code highlight style is configurable the following entry in `_config.yaml`:

```yaml
syntax_highlighter_style: colorful
```

The default code highlight style is `colorful`, the full supported styles can be found from [the rouge repository][6]. Customized
style can be added to [./assets/gitbook/rouge/](./assets/gitbook/rouge/).

## How to generate TOC

The jekyll-gitbook theme leverages [jekyll-toc][4] to generate the *Contents* for the page.
The TOC feature is not enabled by default. To use the TOC feature, modify the TOC
configuration in `_config.yml`:

```yaml
toc:
    enabled: true
    h_min: 1
    h_max: 3
```

## Google Analytics, etc.

The jekyll-gitboook theme supports embedding the [Google Analytics][7], [CNZZ][8] and [Application Insights][9] website analytical tools with the following
minimal configuration in `_config.yaml`:

```yaml
tracker:
  google_analytics: "<YOUR GOOGLE ANALYTICS KEY, e.g, UA-xxxxxx-x>"
```

Similarly, CNZZ can be added with the following configuration in `_config.yaml`

```yaml
tracker:
  cnzz: "<YOUR CNZZ ANALYTICS KEY, e.g., xxxxxxxx>"
```

Application Insights can be added with the following configuration in `_config.yaml`

```yaml
tracker:
  application_insights: "<YOUR APPLICATION INSIGHTS CONNECTION STRING>"
```

## Disqus comments

[Disqus](https://disqus.com/) comments can be enabled by adding the following configuration in `_config.yaml`:

```yaml
disqushandler: "<YOUR DISQUS SHORTNAME>"
```

## Extra StyleSheet or Javascript elements

You can add extra CSS or JavaScript references using configuration collections:

- extra_css: for additional style sheets. If the url does not start by http, the path must be relative to the root of the site, without a starting `/`.
- extra_header_js: for additional scripts to be included in the `<head>` tag, after the `extra_css` has been added. If the url does not start by http, the path must be relative to the root of the site, without a starting `/`.
- extra_footer_js: for additional scripts to be included at the end of the HTML document, just before the site tracking script. If the url does not start by http, the path must be relative to the root of the site, without a starting `/`.

## Customizing font settings

The fonts can be customized by modifying the `.book.font-family-0` and `.book.font-family-1` entry in [`./assets/gitbook/custom.css`][10],

```css
.book.font-family-0 {
    font-family: Georgia, serif;
}
.book.font-family-1 {
    font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
}
```

## Tips, Warnings and Dangers blocks

The jekyll-gitbook theme supports customized kramdown attributes (`{: .block-tip }`, `{: .block-warning }`,
`{: .block-danger }`) like that displayed in [the discord.js website][11]. The marker can be used like

```markdown
> ##### TIP
>
> This guide is last tested with @napi-rs/canvas^0.1.20, so make sure you have
> this or a similar version after installation.
{: .block-tip }
```

Rendered page can be previewed from

[https://sighingnow.github.io/jekyll-gitbook/jekyll/2022-06-30-tips_warnings_dangers.html](https://sighingnow.github.io/jekyll-gitbook/jekyll/2022-06-30-tips_warnings_dangers.html)

## Cover image inside pages

The jekyll-gitbook theme supports adding a cover image to a specific page by adding
a `cover` field to the page metadata:

```diff
  ---
  title: Page with cover image
  author: Tao He
  date: 2022-05-24
  category: Jekyll
  layout: post
+ cover: /assets/jekyll-gitbook/dinosaur.gif
  ---
```

The effect can be previewed from

[https://sighingnow.github.io/jekyll-gitbook/jekyll/2022-05-24-page_cover.html](https://sighingnow.github.io/jekyll-gitbook/jekyll/2022-05-24-page_cover.html)

## Diagrams with mermaid.js

This jekyll-theme supports [mermaid.js](https://mermaid.js.org/) to render diagrams
in markdown.

To enable the mermaid support, you need to set `mermaid: true` in the front matter
of your post.

```markdown
---
mermaid: true
---
```

The example can be previewed from

[https://sighingnow.github.io/jekyll-gitbook/jekyll/2023-08-31-mermaid.html](https://sighingnow.github.io/jekyll-gitbook/jekyll/2023-08-31-mermaid.html)

## License

This work is open sourced under the Apache License, Version 2.0.

Copyright 2019 Tao He.

[1]: finol.official@gmail.com
[2]: https://pages.github.com/themes
[3]: https://github.com/sighingnow/jekyll-gitbook/fork
[4]: https://github.com/allejo/jekyll-toc
[5]: https://github.com/gitbook-plugins/gitbook-plugin-search-pro
[6]: https://github.com/rouge-ruby/rouge/tree/master/lib/rouge/themes
[7]: https://analytics.google.com/analytics/web/
[8]: https://www.cnzz.com/
[9]: https://docs.microsoft.com/en-us/azure/azure-monitor/app/app-insights-overview
[10]: https://github.com/sighingnow/jekyll-gitbook/blob/master/gitbook/custom.css
[11]: https://discordjs.guide/popular-topics/canvas.html#setting-up-napi-rs-canvas
[12]: https://rubygems.org/gems/jekyll-remote-theme
[13]: https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/adding-a-theme-to-your-github-pages-site-using-jekyll
[14]: https://github.com/sighingnow/jekyll-gitbook/blob/master/_config.yml
