<div class="Box-sc-g0xbh4-0 bJMeLZ js-snippet-clipboard-copy-unpositioned" data-hpc="true"><article class="markdown-body entry-content container-lg" itemprop="text"><div align="center" dir="auto">
<div class="markdown-heading" dir="auto"><h1 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">网络每千次展示费用</font></font></h1><a id="user-content-webcpm" class="anchor" aria-label="永久链接：WebCPM" href="#webcpm"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
</div>
<p dir="auto"><font style="vertical-align: inherit;"><a href="https://arxiv.org/abs/2305.06849" rel="nofollow"><font style="vertical-align: inherit;">✨ 这是ACL 2023论文《中文长篇问答互动网络搜索》</font></a><font style="vertical-align: inherit;">的实现</font></font><a href="https://arxiv.org/abs/2305.06849" rel="nofollow"><font style="vertical-align: inherit;"></font></a></p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="/thunlp/WebCPM/blob/main/assets/paper.png"><img src="/thunlp/WebCPM/raw/main/assets/paper.png" alt="纸" style="max-width: 100%;"></a></p>
<p dir="auto"><em><font style="vertical-align: inherit;"></font><a href="/thunlp/WebCPM/blob/main/README_zh.md"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">请用中文</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">阅读此内容</font><font style="vertical-align: inherit;">。</font></font></em></p>
<hr>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">快速链接</font></font></h2><a id="user-content-quick-links" class="anchor" aria-label="永久链接：快速链接" href="#quick-links"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<ul dir="auto">
<li><a href="#quick-links"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">快速链接</font></font></a></li>
<li><a href="#overview"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">概述</font></font></a></li>
<li><a href="#requirements"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">要求</font></font></a></li>
<li><a href="#preparation"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">准备</font></font></a>
<ul dir="auto">
<li><a href="#prepare-the-data"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">准备数据</font></font></a></li>
<li><a href="#prepare-the-model"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">准备模型</font></font></a></li>
</ul>
</li>
<li><a href="#train-webcpm"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">培训网络每千次展示费用</font></font></a>
<ul dir="auto">
<li><a href="#a-brief-introduction-of-pipeline-based-web-search"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">基于管道的Web搜索简介</font></font></a></li>
<li><a href="#data-preprocessing"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">数据预处理</font></font></a>
<ul dir="auto">
<li><a href="#training-data-generation-of-interactive-web-search"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">交互式网络搜索的训练数据生成</font></font></a></li>
<li><a href="#training-data-generation-of-pipeline-based-web-search"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">基于管道的网络搜索的训练数据生成</font></font></a></li>
</ul>
</li>
<li><a href="#training"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">训练</font></font></a></li>
</ul>
</li>
<li><a href="#single-task-evaluation"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">单任务评估</font></font></a></li>
<li><a href="#run-webcpm-for-new-questions"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">针对新问题运行 WebCPM</font></font></a>
<ul dir="auto">
<li><a href="#interactive-web-search"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">交互式网络搜索</font></font></a></li>
<li><a href="#pipeline-based-web-search"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">基于管道的网络搜索</font></font></a></li>
</ul>
</li>
<li><a href="#platform-building-for-data-annotation"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">数据标注平台搭建</font></font></a></li>
<li><a href="#bugs-or-questions"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">错误或问题？</font></font></a></li>
<li><a href="#resources-of-tool-learning"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">工具学习资源</font></font></a></li>
<li><a href="#citation"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">引文</font></font></a></li>
</ul>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">概述</font></font></h2><a id="user-content-overview" class="anchor" aria-label="永久链接：概述" href="#overview"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="/thunlp/WebCPM/blob/main/assets/platform.png"><img src="/thunlp/WebCPM/raw/main/assets/platform.png" alt="平台" style="max-width: 100%;"></a></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">在这项工作中，我们提出了 WebCPM，一个使用中文预训练模型进行交互式网络搜索的项目。我们开发了一个网络搜索界面，它既适合人类，又收集人类的网络搜索行为。然后，我们使用多达 10B 个参数对 PLM 进行微调，以模仿人类的网络搜索行为，并根据收集到的事实生成答案。我们开源网络搜索接口、数据集、实现和模型参数。</font></font></p>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">要求</font></font></h2><a id="user-content-requirements" class="anchor" aria-label="永久链接：要求" href="#requirements"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">要运行我们的代码，请使用以下命令安装所有依赖包：</font></font></p>
<div class="snippet-clipboard-content notranslate position-relative overflow-auto"><pre class="notranslate"><code>pip install -r requirements.txt
</code></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="pip install -r requirements.txt" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto"><strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">注意</font></font></strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">：不同版本的软件包（例如，</font></font><code>pytorch</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">）可能会导致本文得出不同的结果。然而，无论您使用什么版本的软件包，这种趋势应该仍然存在。</font></font></p>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">准备</font></font></h2><a id="user-content-preparation" class="anchor" aria-label="永久链接：准备" href="#preparation"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">准备数据</font></font></h3><a id="user-content-prepare-the-data" class="anchor" aria-label="永久链接：准备数据" href="#prepare-the-data"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"></font><a href="https://drive.google.com/drive/folders/1IQBOCwhcMUnkxevv9wVFVLIFT3o8f7HX?usp=sharing" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">首先从Google Drive</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">下载数据</font><font style="vertical-align: inherit;">，并将文件</font></font><code>interactive_data</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">和</font></font><code>pipeline_data</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">放到</font></font><code>./data</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">，或者运行以下命令：</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">下载的文件包含以下内容：</font></font></p>
<p dir="auto"><code>interactive_data/data.json</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">是论文实验中使用的数据集（</font><font style="vertical-align: inherit;">总共
</font></font><strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">5500个</font></font></strong><font style="vertical-align: inherit;"></font><code>interactive_data/data_zhihu.json</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">实例）。是与本文一起收集的附加数据集（约</font></font><strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">900 个</font></font></strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">实例），问题来自知乎</font></font><a href="https://www.zhihu.com/people/71-26-1-50" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">，</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">您可以使用它来进行数据增强。</font></font></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">请使用以下代码将上述数据拆分为train、dev和test集（设置--add_zhihu将添加data_zhihu.json）。</font></font></p>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre><span class="pl-c1">cd</span> data/interactive_data
python split.py --add_zhihu</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="cd data/interactive_data
python split.py --add_zhihu" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">除了交互式网络搜索数据之外，我们还提供了训练基于管道的网络搜索所需的数据集：（</font></font><code>pipeline_data</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">总共</font><font style="vertical-align: inherit;">110k 个实例）</font></font><strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font></font></strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">所有数据都是通过提示text-davinci-003（也涉及Bing搜索引擎）创建的，然后由人工注释者手动过滤。 （</font></font><strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">注意</font></font></strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">这部分没有包含在论文中，不需要将其拆分为train / dev / test。）</font></font></p>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">准备模型</font></font></h3><a id="user-content-prepare-the-model" class="anchor" aria-label="永久链接：准备模型" href="#prepare-the-model"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">WebCPM基于</font></font><a href="https://github.com/OpenBMB/CPM-Live"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">CPM-bee</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;"> ，参数高达</font></font><strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">100亿</font></font></strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">，是社区最大的中文预训练语言模型之一。我们使用 CPM-bee 的早期版本，表示为 cpm_10b_webcpm_exp.pt。最新版本的 CPM-bee 托管在</font></font><a href="https://github.com/OpenBMB/CPM-Bee"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">New-CPM-bee</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。您可能需要替换新版本的 cpm-live 软件包。</font></font><strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">请注意，模型检查点尚未针对任何下游任务进行微调</font></font></strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。要访问cpm_10b_webcpm_exp.pt，您可以在</font></font><a href="https://cloud.tsinghua.edu.cn/d/a02ae00b11434c9c8560/" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">清华云</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">下载模型参数</font><font style="vertical-align: inherit;">，或运行以下脚本：</font></font></p>
<div class="snippet-clipboard-content notranslate position-relative overflow-auto"><pre class="notranslate"><code>cd models
bash download_model_initial_model.sh
</code></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="cd models
bash download_model_initial_model.sh" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">上述代码会在 处下载10B（非微调）模型</font></font><code>models</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">，微调后的管道模型请参考，或从</font><a href="https://cloud.tsinghua.edu.cn/d/3dc39eccc6c64bb58671/" rel="nofollow"><font style="vertical-align: inherit;">清华云</font></a></font><code>download_model_pipeline_finetuned.sh</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">手动下载</font><font style="vertical-align: inherit;">。</font></font><a href="https://cloud.tsinghua.edu.cn/d/3dc39eccc6c64bb58671/" rel="nofollow"><font style="vertical-align: inherit;"></font></a><font style="vertical-align: inherit;"></font></p>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">培训网络每千次展示费用</font></font></h2><a id="user-content-train-webcpm" class="anchor" aria-label="永久链接：训练 WebCPM" href="#train-webcpm"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="/thunlp/WebCPM/blob/main/assets/framework.png"><img src="/thunlp/WebCPM/raw/main/assets/framework.png" alt="平台" style="max-width: 100%;"></a></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">我们提供了两个版本的WebCPM：（1）交互式网络搜索（ACL论文中提出的方法）和（2）基于管道的网络搜索，更容易部署（论文中没有报道该方法）。两个版本都使用不同的脚本来生成训练数据，并使用相同的代码来进行模型训练。</font></font></p>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">基于管道的Web搜索简介</font></font></h3><a id="user-content-a-brief-introduction-of-pipeline-based-web-search" class="anchor" aria-label="永久链接：基于管道的 Web 搜索简介" href="#a-brief-introduction-of-pipeline-based-web-search"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">工作流程分为四个阶段：（1）首先，根据原始问题生成可能的搜索查询； (2)然后对于每个搜索查询，调用Bing搜索并访问top-K网页； (3)针对每个网页，提取重要信息； (4) 根据所有记录的信息，生成连贯且细致入微的答案。所有这些都是以多任务方式训练的，请参考</font></font><code>run_web_browsing/run_pipeline.py</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。有关交互式网络搜索的详细信息，请参阅我们的原始论文。</font></font></p>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">数据预处理</font></font></h3><a id="user-content-data-preprocessing" class="anchor" aria-label="永久链接：数据预处理" href="#data-preprocessing"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">在开始之前，请运行以下代码：</font></font></p>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre><span class="pl-k">export</span> PYTHONPATH=/<span class="pl-k">**</span>your-base-path<span class="pl-k">**</span>/webcpm</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="export PYTHONPATH=/**your-base-path**/webcpm" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">训练数据生成如下（我们区分交互式网络搜索和基于管道的方法）。以下代码会在对应文件夹中生成</font></font><code>train_data</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">、</font></font><code>dev_data</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">、</font></font><code>test_data</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">，训练时会加载。</font></font></p>
<div class="markdown-heading" dir="auto"><h4 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">交互式网络搜索的训练数据生成</font></font></h4><a id="user-content-training-data-generation-of-interactive-web-search" class="anchor" aria-label="永久链接：交互式网络搜索的训练数据生成" href="#training-data-generation-of-interactive-web-search"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">首先，使用以下代码构建综合模型的数据：</font></font></p>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre><span class="pl-c1">cd</span> dataset_interactive
python make_data_synthesis_model.py --data_path ../../data/interactive_data  --augment_qa_data --augment_data_path ../../data/pipeline_data</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="cd dataset_interactive
python make_data_synthesis_model.py --data_path ../../data/interactive_data  --augment_qa_data --augment_data_path ../../data/pipeline_data" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">我们对一些论点的解释如下：</font></font></p>
<ul dir="auto">
<li><code>data_path</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">：源数据路径。</font></font></li>
<li><code>augment_qa_data</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">：是否使用text-davinci自动生成的qa数据来增强训练数据。 （要复制我们论文中的结果，请不要添加此参数）</font></font></li>
<li><code>augment_data_path</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">：增强训练数据的数据路径。</font></font></li>
</ul>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">搜索模型的训练数据生成如下：</font></font></p>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre>python make_data_search_model.py --add_query --add_action --add_abstract --abstract_all_tokens</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="python make_data_search_model.py --add_query --add_action --add_abstract --abstract_all_tokens" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">我们对一些论点的解释如下：</font></font></p>
<ul dir="auto">
<li><code>data_path</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">：源数据路径。</font></font></li>
<li><code>add_query</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">：如果为True，将添加查询生成数据。</font></font></li>
<li><code>add_abstract</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">：如果为 True，将添加生成支持事实提取数据。</font></font></li>
<li><code>abstract_all_tokens</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">：如果为 True，则支持事实提取模块将生成所有标记，而不是仅生成前/最后几个标记。</font></font></li>
<li><code>add_action</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">：如果为 True，将添加动作预测数据。</font></font></li>
<li><code>add_synthesis</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">：如果为 True，将为综合模型加载本地数据。</font></font><strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">注意 您必须首先运行 python make_data_synthesis_model.py 来获取综合数据，然后在此处添加此参数</font></font></strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。</font></font></li>
</ul>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">如果你想以多任务的方式训练所有子任务，只需添加以上所有参数即可；否则只</font></font><code>--add_query</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">为单任务测试</font><font style="vertical-align: inherit;">添加一个参数（例如， ）。</font></font></p>
<div class="markdown-heading" dir="auto"><h4 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">基于管道的网络搜索的训练数据生成</font></font></h4><a id="user-content-training-data-generation-of-pipeline-based-web-search" class="anchor" aria-label="永久链接：基于管道的网络搜索的训练数据生成" href="#training-data-generation-of-pipeline-based-web-search"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">请运行以下代码：</font></font></p>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre><span class="pl-c1">cd</span> dataset_pipeline
python make_data.py</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="cd dataset_pipeline
python make_data.py" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">训练</font></font></h3><a id="user-content-training" class="anchor" aria-label="永久链接：培训" href="#training"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">要训&ZeroWidthSpace;&ZeroWidthSpace;练 WebCPM，请运行以下代码：</font></font></p>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre><span class="pl-c1">cd</span> training
<span class="pl-k">export</span> PYTHONPATH=/<span class="pl-k">**</span>your-base-path<span class="pl-k">**</span>/webcpm
<span class="pl-k">export</span> CUDA_VISIBLE_DEVICES=0,1,2,3,4,5,6,7
GPUS_PER_NODE=<span class="pl-s"><span class="pl-pds">$(</span>echo <span class="pl-smi">$CUDA_VISIBLE_DEVICES</span> <span class="pl-k">|</span> tr <span class="pl-s"><span class="pl-pds">'</span>,<span class="pl-pds">'</span></span> <span class="pl-s"><span class="pl-pds">'</span>\n<span class="pl-pds">'</span></span> <span class="pl-k">|</span> wc -l <span class="pl-k">|</span> xargs<span class="pl-pds">)</span></span>
<span class="pl-c1">echo</span> <span class="pl-s"><span class="pl-pds">"</span>Number of visible devices: <span class="pl-smi">$GPUS_PER_NODE</span>, should be the same as visible devices<span class="pl-pds">"</span></span>

<span class="pl-c1">set</span> -ex

MASTER_ADDR=localhost
MASTER_PORT=3239
NNODES=1
NODE_RANK=0

OPTS=<span class="pl-s"><span class="pl-pds">"</span><span class="pl-pds">"</span></span>
OPTS+=<span class="pl-s"><span class="pl-pds">"</span> --model-config config/cpm-bee-10b.json<span class="pl-pds">"</span></span>
OPTS+=<span class="pl-s"><span class="pl-pds">"</span> --dataset ../data/dataset_interactive/train_data<span class="pl-pds">"</span></span>
OPTS+=<span class="pl-s"><span class="pl-pds">"</span> --dataseteval ../data/dataset_interactive/dev_data<span class="pl-pds">"</span></span>
OPTS+=<span class="pl-s"><span class="pl-pds">"</span> --epoch 5<span class="pl-pds">"</span></span>
OPTS+=<span class="pl-s"><span class="pl-pds">"</span> --batch-size 8<span class="pl-pds">"</span></span>
OPTS+=<span class="pl-s"><span class="pl-pds">"</span> --train-iters 100<span class="pl-pds">"</span></span>
OPTS+=<span class="pl-s"><span class="pl-pds">"</span> --save-name webcpm_finetuned<span class="pl-pds">"</span></span>
OPTS+=<span class="pl-s"><span class="pl-pds">"</span> --max-length 2560<span class="pl-pds">"</span></span>
OPTS+=<span class="pl-s"><span class="pl-pds">"</span> --save ../models/<span class="pl-pds">"</span></span>
OPTS+=<span class="pl-s"><span class="pl-pds">"</span> --lr 0.0001<span class="pl-pds">"</span></span>
OPTS+=<span class="pl-s"><span class="pl-pds">"</span> --inspect-iters 100<span class="pl-pds">"</span></span>
OPTS+=<span class="pl-s"><span class="pl-pds">"</span> --warmup-iters 1<span class="pl-pds">"</span></span>
OPTS+=<span class="pl-s"><span class="pl-pds">"</span> --save-epochs 1<span class="pl-pds">"</span></span>
OPTS+=<span class="pl-s"><span class="pl-pds">"</span> --lr-decay-style noam<span class="pl-pds">"</span></span>
OPTS+=<span class="pl-s"><span class="pl-pds">"</span> --weight-decay 0.01<span class="pl-pds">"</span></span>
OPTS+=<span class="pl-s"><span class="pl-pds">"</span> --clip-grad 1.0<span class="pl-pds">"</span></span>
OPTS+=<span class="pl-s"><span class="pl-pds">"</span> --loss-scale 32768<span class="pl-pds">"</span></span>
OPTS+=<span class="pl-s"><span class="pl-pds">"</span> --start-step 0<span class="pl-pds">"</span></span>
OPTS+=<span class="pl-s"><span class="pl-pds">"</span> --load ../models/cpm_10b_webcpm_exp.pt<span class="pl-pds">"</span></span>

CMD=<span class="pl-s"><span class="pl-pds">"</span>torchrun --nnodes=<span class="pl-smi">${NNODES}</span> --nproc_per_node=<span class="pl-smi">${GPUS_PER_NODE}</span> --rdzv_id=1 --rdzv_backend=c10d --rdzv_endpoint=<span class="pl-smi">${MASTER_ADDR}</span>:<span class="pl-smi">${MASTER_PORT}</span> finetune_cpm_bee.py <span class="pl-smi">${OPTS}</span><span class="pl-pds">"</span></span>

<span class="pl-c1">echo</span> <span class="pl-smi">${CMD}</span>
<span class="pl-smi">$CMD</span></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="cd training
export PYTHONPATH=/**your-base-path**/webcpm
export CUDA_VISIBLE_DEVICES=0,1,2,3,4,5,6,7
GPUS_PER_NODE=$(echo $CUDA_VISIBLE_DEVICES | tr ',' '\n' | wc -l | xargs)
echo &quot;Number of visible devices: $GPUS_PER_NODE, should be the same as visible devices&quot;

set -ex

MASTER_ADDR=localhost
MASTER_PORT=3239
NNODES=1
NODE_RANK=0

OPTS=&quot;&quot;
OPTS+=&quot; --model-config config/cpm-bee-10b.json&quot;
OPTS+=&quot; --dataset ../data/dataset_interactive/train_data&quot;
OPTS+=&quot; --dataseteval ../data/dataset_interactive/dev_data&quot;
OPTS+=&quot; --epoch 5&quot;
OPTS+=&quot; --batch-size 8&quot;
OPTS+=&quot; --train-iters 100&quot;
OPTS+=&quot; --save-name webcpm_finetuned&quot;
OPTS+=&quot; --max-length 2560&quot;
OPTS+=&quot; --save ../models/&quot;
OPTS+=&quot; --lr 0.0001&quot;
OPTS+=&quot; --inspect-iters 100&quot;
OPTS+=&quot; --warmup-iters 1&quot;
OPTS+=&quot; --save-epochs 1&quot;
OPTS+=&quot; --lr-decay-style noam&quot;
OPTS+=&quot; --weight-decay 0.01&quot;
OPTS+=&quot; --clip-grad 1.0&quot;
OPTS+=&quot; --loss-scale 32768&quot;
OPTS+=&quot; --start-step 0&quot;
OPTS+=&quot; --load ../models/cpm_10b_webcpm_exp.pt&quot;

CMD=&quot;torchrun --nnodes=${NNODES} --nproc_per_node=${GPUS_PER_NODE} --rdzv_id=1 --rdzv_backend=c10d --rdzv_endpoint=${MASTER_ADDR}:${MASTER_PORT} finetune_cpm_bee.py ${OPTS}&quot;

echo ${CMD}
$CMD" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">我们对一些论点的解释如下：</font></font></p>
<ul dir="auto">
<li><code>dataset</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">和</font></font><code>dataseteval</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">：已处理文件的路径。对于交互式网络搜索，它是dataset_interactive，而对于基于管道的方法，它是dataset_pipeline。</font></font></li>
<li><code>batch-size</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">：单个GPU的批量大小，实际批量大小将为#GPUs x 每个GPU的批量大小。</font></font></li>
<li><code>max-length</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">：数据（不是模型）的最大序列长度，那些较长的训练实例将被丢弃。</font></font></li>
<li><code>save-name</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">和</font></font><code>save</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">：保存微调模型的路径和保存的模型检查点的名称。</font></font></li>
<li><code>epoch</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">：训练时期数。</font></font></li>
<li><code>load</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">：预训练模型检查点的路径（在本例中为 cpmb）。</font></font></li>
</ul>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">请注意，无论您正在训练哪个模块（或多任务设置），都可以使用上述代码。我们在8x80G A100上进行训练，您可以根据您的GPU设备更改batch size，性能对超参数不敏感。</font></font></p>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">单任务评估</font></font></h2><a id="user-content-single-task-evaluation" class="anchor" aria-label="永久链接：单任务评估" href="#single-task-evaluation"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">要评估不同的子任务，您可以首先运行以下代码来获得微调模型对测试数据的预测：</font></font></p>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre><span class="pl-c1">cd</span> inference
python inference.py --test_file ../training/dataset_interactive/test.txt --output_file output/test_predictions.json --ckpt_path <span class="pl-k">**</span>your_finetuned_checkpoint.pt</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="cd inference
python inference.py --test_file ../training/dataset_interactive/test.txt --output_file output/test_predictions.json --ckpt_path **your_finetuned_checkpoint.pt" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">我们对一些论点的解释如下：</font></font></p>
<ul dir="auto">
<li><code>test_file</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">：测试文件的路径，应该是数据预处理时生成的。</font></font></li>
<li><code>output_file</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">：您要写入预测的路径。</font></font></li>
<li><code>ckpt_path</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">：微调模型的路径。</font></font></li>
</ul>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">获得测试文件的预测后，可以运行以下代码进行单任务评估：</font></font></p>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre>python evaluate.py --input_file output/test_predictions.txt --evaluate_action</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="python evaluate.py --input_file output/test_predictions.txt --evaluate_action" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">我们对一些论点的解释如下：</font></font></p>
<ul dir="auto">
<li><code>input_file</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">：您编写测试文件的预测的路径。</font></font></li>
<li><code>evaluate_action</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">：是否要评估动作预测任务（F1）。</font></font></li>
<li><code>evaluate_query</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">：是否要评估搜索查询生成任务（Rougel-L）。</font></font></li>
<li><code>evaluate_abstract</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">：是否要评估支持事实提取任务（Rougel-L）。</font></font></li>
<li><code>abstract_all_tokens</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">：您使用哪种模式来训练模型以支持事实提取，如果生成所有标记，请添加此参数（Rougel-L）。</font></font></li>
<li><code>evaluate_answer</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">：是否要评估答案综合任务（Rougel-L）。</font></font></li>
<li><code>beam_size</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">：将光束大小设置为 1 会显着加速推理，但会稍微损害性能。</font></font></li>
</ul>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">针对新问题运行 WebCPM</font></font></h2><a id="user-content-run-webcpm-for-new-questions" class="anchor" aria-label="永久链接：针对新问题运行 WebCPM" href="#run-webcpm-for-new-questions"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">这是整个管道评估的实现。您可以使用以下代码生成新问题的答案。请注意，这要求您首先从</font></font><a href="https://www.microsoft.com/en-us/bing/apis/bing-web-search-api" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">此处</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">获取 Bing 搜索 API 密钥</font><font style="vertical-align: inherit;">并运行以下代码：</font></font></p>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre><span class="pl-c1">cd</span> run_web_browsing
<span class="pl-k">export</span> PYTHONPATH=/<span class="pl-k">**</span>base-path<span class="pl-k">**</span>/webcpm
<span class="pl-k">export</span> BING_SEARCH_KEY=<span class="pl-s"><span class="pl-pds">"</span>**Your Bing Search API Key**<span class="pl-pds">"</span></span></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="cd run_web_browsing
export PYTHONPATH=/**base-path**/webcpm
export BING_SEARCH_KEY=&quot;**Your Bing Search API Key**&quot;" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">交互式网络搜索</font></font></h3><a id="user-content-interactive-web-search" class="anchor" aria-label="永久链接：交互式网络搜索" href="#interactive-web-search"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre>python run_interactive.py --data_path predictions/test_interactive.json --ckpt_path <span class="pl-k">**</span>your-checkpoint<span class="pl-k">**</span></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="python run_interactive.py --data_path predictions/test_interactive.json --ckpt_path **your-checkpoint**" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<div class="markdown-heading" dir="auto"><h3 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">基于管道的网络搜索</font></font></h3><a id="user-content-pipeline-based-web-search" class="anchor" aria-label="永久链接：基于管道的网络搜索" href="#pipeline-based-web-search"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<div class="highlight highlight-source-shell notranslate position-relative overflow-auto" dir="auto"><pre>python run_pipeline.py --data_path predictions/test.json --ckpt_path <span class="pl-k">**</span>your-checkpoint<span class="pl-k">**</span></pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="python run_pipeline.py --data_path predictions/test.json --ckpt_path **your-checkpoint**" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">我们对一些论点的解释如下：</font></font></p>
<ul dir="auto">
<li><code>data_path</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">：您编写预测的路径。</font></font></li>
<li><code>ckpt_path</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">：使用基于管道的方法进行训练的检查点的路径。</font></font></li>
</ul>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">数据标注平台搭建</font></font></h2><a id="user-content-platform-building-for-data-annotation" class="anchor" aria-label="永久链接：数据注释平台构建" href="#platform-building-for-data-annotation"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="/thunlp/WebCPM/blob/main/assets/annotation.png"><img src="/thunlp/WebCPM/raw/main/assets/annotation.png" alt="平台" style="max-width: 100%;"></a></p>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">我们开源了我们的网络搜索接口，您可以使用它来进行数据注释。请参阅</font></font><a href="/thunlp/WebCPM/blob/main/annotation_platform/README.md"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">注释</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。目前代码有点混乱，我们很快就会上传更清晰的版本。</font></font></p>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">错误或问题？</font></font></h2><a id="user-content-bugs-or-questions" class="anchor" aria-label="永久链接：错误或问题？" href="#bugs-or-questions"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">如果您对代码或论文有任何疑问，请联系 Yujia ( </font></font><code>qyj20@mails.tsinghua.edu.cn</code><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">) 或提出问题。</font></font></p>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">工具学习资源</font></font></h2><a id="user-content-resources-of-tool-learning" class="anchor" aria-label="永久链接：工具学习资源" href="#resources-of-tool-learning"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">凭借基础模型的强大功能，我们渴望看到它们在操作各种工具方面的应用。 WebCPM就是一种典型的研究尝试。更多资源请参考以下内容：</font></font></p>
<ul dir="auto">
<li>
<p dir="auto"><strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">BM工具</font></font></strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。 [</font></font><a href="https://github.com/OpenBMB/BMTools"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">项目</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">]</font></font></p>
</li>
<li>
<p dir="auto"><strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">工具学习</font></font></strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。 [</font></font><a href="https://arxiv.org/abs/2304.08354" rel="nofollow"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">纸</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">]</font></font></p>
</li>
<li>
<p dir="auto"><strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">工具学习论文列表</font></font></strong><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">。 [</font></font><a href="https://github.com/thunlp/ToolLearningPapers"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">项目</font></font></a><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">]</font></font></p>
</li>
</ul>
<div class="markdown-heading" dir="auto"><h2 tabindex="-1" class="heading-element" dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">引文</font></font></h2><a id="user-content-citation" class="anchor" aria-label="永久链接：引文" href="#citation"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="auto"><font style="vertical-align: inherit;"><font style="vertical-align: inherit;">如果您发现我们的 WebCPM 有用，请使用以下引用：</font></font></p>
<div class="highlight highlight-text-bibtex notranslate position-relative overflow-auto" dir="auto"><pre><span class="pl-k">@inproceedings</span>{<span class="pl-en">qin2023webcpm</span>,
    <span class="pl-s">title</span> = <span class="pl-s"><span class="pl-pds">"</span>WebCPM: Interactive Web Search for Chinese Long-form Question Answering<span class="pl-pds">"</span></span>,
    <span class="pl-s">author</span>=<span class="pl-s"><span class="pl-pds">{</span>Yujia Qin and Zihan Cai and Dian Jin and Lan Yan and Shihao Liang and Kunlun Zhu and Yankai Lin and Xu Han and Ning Ding and Huadong Wang and Ruobing Xie and Fanchao Qi and Zhiyuan Liu and Maosong Sun and Jie Zhou<span class="pl-pds">}</span></span>,
    <span class="pl-s">booktitle</span> = <span class="pl-s"><span class="pl-pds">"</span>Proceedings of ACL 2023<span class="pl-pds">"</span></span>,
    <span class="pl-s">year</span> = <span class="pl-s"><span class="pl-pds">"</span>2023<span class="pl-pds">"</span></span>,
    <span class="pl-s">publisher</span> = <span class="pl-s"><span class="pl-pds">"</span>Association for Computational Linguistics<span class="pl-pds">"</span></span>,
    <span class="pl-s">url</span> = <span class="pl-s"><span class="pl-pds">"</span>https://arxiv.org/abs/2305.06849<span class="pl-pds">"</span></span>,
}</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 tooltipped-no-delay d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="@inproceedings{qin2023webcpm,
    title = &quot;WebCPM: Interactive Web Search for Chinese Long-form Question Answering&quot;,
    author={Yujia Qin and Zihan Cai and Dian Jin and Lan Yan and Shihao Liang and Kunlun Zhu and Yankai Lin and Xu Han and Ning Ding and Huadong Wang and Ruobing Xie and Fanchao Qi and Zhiyuan Liu and Maosong Sun and Jie Zhou},
    booktitle = &quot;Proceedings of ACL 2023&quot;,
    year = &quot;2023&quot;,
    publisher = &quot;Association for Computational Linguistics&quot;,
    url = &quot;https://arxiv.org/abs/2305.06849&quot;,
}" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
</article></div>
