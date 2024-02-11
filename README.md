[![Python 3.9](https://shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-3916/)
[![Platform](https://img.shields.io/badge/platform-linux%20%7C%20windows%20%7C%20macos-lightgrey)](Platform)
[![License](https://img.shields.io/github/license/jiahaoli57/FinOL)](License)
[![Document](https://img.shields.io/badge/docs-latest-red)](https://finol.readthedocs.io/en/latest/)

[![](https://dcbadge.vercel.app/api/server/3tEwzBBT)](https://discord.gg/3tEwzBBT)

[//]: # ([![GitHub stars]&#40;https://img.shields.io/github/stars/ai4finol/finol?color=orange&#41;]&#40;https://github.com/ai4finol/finol/stargazers&#41;)


``FinOL`` represents a pioneering open database for facilitating data-driven financial research. As an
ambitious project, it collects and organizes extensive assets from global markets over half a century,
it provides a long-awaited unified platform to advance data-driven OLPS research.

## About

Online portfolio selection (OLPS) is an important issue in operations research community that studies how to dynamically
adjust portfolios according to market changes. In the past, OLPS research relied on a general database called ``OLPS`` 
containing price relatives data of financial assets across different markets. However, with the widespread adoption of 
data-driven technologies like machine learning in finance, ``OLPS`` can no longer meet the needs of OLPS research because 
due to the lack of support for complex data types, high-dimensional feature spaces, and multi-source data fusion. To solve 
this problem, we propose ``FinOL``, an open finance database for advancing research in data-driven OLPS. ``FinOL`` expands 
and enriches the previous ``OLPS`` database, containing 8 benchmark financial datasets from 1962 to present across global 
markets. To promote fair comparisons, we evaluate a large number of past classic OLPS methods on ``FinOL``, providing 
reusable benchmark results for future ``FinOL`` users and effectively supporting OLPS research. Importantly, we are 
committed to regularly updating ``FinOL`` with new data and benchmark results reflecting the latest developments and 
trends in the field. This ensures ``FinOL`` remains a valuable resource as data-driven OLPS methods continue evolving.

## Contact Us

For inquiries, please get in touch with us at [finol.official@gmail.com](mailto:finol.official@gmail.com) (Monday to Friday, 9:00 AM to 6:00 PM)

<!-- ## Benchmark Results of Daily Cumulative Wealth

{% raw %}
<div id="main" style="width: 900px;height:400px;"></div>

<script type="text/javascript">
  // 在这里编写你的 ECharts 图表代码
  // 例如：
  var ROOT_PATH = 'https://ai4finol.github.io';
  var chartDom = document.getElementById('main');
  var myChart = echarts.init(chartDom);
  var option;

  $.get(
    ROOT_PATH + '/assets/dcw.json',
    function (_rawData) {
      run(_rawData);
    }
  );

  function run(_rawData) {
    var strategies = [
      'Market', 'Best', 'UCRP', 'BCRP', 'UP',
      'EG', 'SCRP', 'PPT', 'ANTI1', 'ANTI2', 'PAMR'
    ];

    var dataset = strategies.map(function (strategy) {
      return {
        id: 'dataset_of_' + strategy,
        fromDatasetId: 'dataset_raw',
        transform: {
          type: 'filter',
          config: {
            and: [
              { dimension: 'Strategy', '=': strategy }
            ]
          }
        }
      };
    });

    dataset.unshift({
      id: 'dataset_raw',
      source: _rawData
    });
    
    var series = strategies.map(function (strategy) {
      return {
        name: strategy,
        type: 'line',
        datasetId: 'dataset_of_' + strategy,
        showSymbol: true,
        encode: {
          x: 'Time',
          y: 'DCW',
          itemName: 'Time',
          tooltip: ['DCW']
        }
      };
    });

    option = {
      dataset: dataset,
      tooltip: {
        trigger: 'axis'
      },
      legend: {
        data: strategies
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
        type: 'category',
        axisLabel: {
          interval: 50 // 每50个显示一个标签
        }
      },
      yAxis: {
        name: 'DCW',
        min: 0.6,  // 设置最小值
      },
      series: series
    };
    myChart.setOption(option);
  }
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

[https://sighingnow.github.io/jekyll-gitbook/jekyll/2023-08-31-mermaid.html](https://sighingnow.github.io/jekyll-gitbook/jekyll/2023-08-31-mermaid.html) -->

<!-- ## License

This work is open sourced under the MIT License.

Copyright 2024 Jiahao Li. -->

<!-- [1]: finol.official@gmail.com
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
[14]: https://github.com/sighingnow/jekyll-gitbook/blob/master/_config.yml -->
