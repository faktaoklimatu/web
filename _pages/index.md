---
layout: empty
title: Fakta o klimatu
slug: index
---
<div class="section intro">
    <div class="container">
        <h1 class="display-1" id="home">Fakta o změně<br>klimatu</h1>
        <span class="tagline">Veřejně dostupné<br>infografiky a datasety</span>
        <p class="mb-5">Shromažďujeme data o klimatu a klimatické změně, která poskytují vědecké instituce (ČHMÚ, NASA, Eurostat a jiné) a zpracováváme z nich grafy a infografiky pro <a href="/jak-pouzivat" title="Jak používat naše materiály">další použití</a>.<br/>
            <a href="{{ site.fundraising }}" class="btn btn-primary mt-3"><i class="fas fa-fw fa-heart"></i> Podpořte nás</a>
            <a href="/aktuality" class="btn btn-secondary mt-3"><i class="fas fa-fw fa-newspaper"></i> Aktuality</a>
            <a href="#o-projektu" class="btn btn-secondary mt-3"><i class="fas fa-fw fa-info"></i> O projektu</a>
        </p>
        <ul class="nav nav-tabs" role="tablist">
            <li class="nav-item" role="presentation">
                <h2 class="nav-link bg-extralight-blue active" id="tab-role-public" data-toggle="tab" href="#public" role="tab" aria-controls="public" aria-selected="true">Pro veřejnost</h2>
            </li>
            <li class="nav-item" role="presentation">
                <h2 class="nav-link bg-extralight-green" id="tab-role-teachers" data-toggle="tab" href="#teachers" role="tab" aria-controls="teachers" aria-selected="false">Pro učitele</h2>
            </li>
            <li class="nav-item" role="presentation">
                <h2 class="nav-link bg-extralight-red" id="tab-role-journalists" data-toggle="tab" href="#journalists" role="tab" aria-controls="journalists" aria-selected="false">Pro novináře</h2>
            </li>
        </ul>
    </div>
</div>

<div class="tab-content" id="myTabContent">
  <div class="section tab-pane fade show active bg-extralight-blue pt-4 pb-4" id="public" role="tabpanel" aria-labelledby="tab-role-public"><div class="container">
    <p class="lead mb-0">Fakta o klimatu neslouží odborníkům, ale všem lidem se zájmem o téma klimatické změny. Pokud jste na našem webu poprvé a nevíte kde začít, můžete si prohlédnout některou z úvodních infografik níže.</p>
    {% assign featured_slugs = "schema-klimaticke-zmeny, emise-cr-detail, koncentrace-co2, body-zlomu-1, teplota-22000-let, teplota-cr, potencial-zpusobu-snizeni-emisi, elektrina-cr" | split: ", " %}
    {% assign featured = site.infographics | where_exp: "item", "featured_slugs contains item.slug" | sample: 3 %}
    {% include preview-blocks.html blocks=featured limit=3 %}
    <p class="lead">Pro pravidelné kvalitní informace o klimatické změně můžete sledovat náš newsletter nebo Twitter.
    Komplexní a přístupný pohled na klimatickou změnu představuje naše publikace <a href="/atlas" target="_blank">Atlas klimatické změny</a>.
    Kvalitní debatu o klimatické změně a projekt Fakta o klimatu můžete také podpořit – finančně nebo používáním našich dat a grafik.</p>
    <a href="#newsletter-modal" class="btn btn-primary" id="newsletter-embed" data-toggle="modal" data-target="#newsletter-modal"><i class="fas fa-fw fa-envelope-open-text"></i> Newsletter</a>
    <a href="https://twitter.com/{{ site.twitter }}" target="_blank" class="btn btn-secondary"><i class="fab fa-fw fa-twitter"></i> Twitter</a>
    <a href="/temata/emise/" class="btn btn-secondary"><i class="fas fa-fw fa-binoculars"></i> Explainery</a>
    <a href="/slovnik" class="btn btn-secondary"><i class="fas fa-fw fa-book"></i> Slovník pojmů</a>
    <a href="/zdroje" class="btn btn-secondary"><i class="fas fa-fw fa-globe"></i> Další zdroje a odkazy</a>
  </div></div>

  <div class="section tab-pane fade bg-extralight-green pt-4 pb-4" id="teachers" role="tabpanel" aria-labelledby="tab-role-teachers"><div class="container">
    <p class="lead mb-0">Texty a grafiky projektu Fakta o klimatu lze použít jako materiál pro přípravu různých vzdělávacích aktivit. Při práci se snažíme nerezignovat na vědeckou přesnost a komplexnost, použití našich textů a grafik proto doporučujeme ve vyšších ročnících ZŠ nebo na SŠ a VŠ. Pokud jste na našem webu poprvé a nevíte kde začít, můžete si prohlédnout některou z úvodních infografik níže.</p>
    {% assign featured_slugs = "schema-klimaticke-zmeny, emise-cr-detail, koncentrace-co2" | split: ", " %}
    {% assign featured = site.infographics | where_exp: "item", "featured_slugs contains item.slug" | sample: 3 %}
    {% include preview-blocks.html blocks=featured limit=3 %}
    <div class="row justify-content-md">
      <div class="col-md-6 col-lg-8">
        <p class="lead">Jazykově a obsahově nejpřístupnější je naše publikace Atlas klimatické změny, která uceleně vysvětluje jevy způsobující nebo provázející klimatickou změnu. Práci s texty a grafikami se snažíme usnadnit pomocí slovníku pojmů a explainerů („vysvětlovačů“).</p>
        <a href="/atlas" class="btn btn-primary" target="_blank"><i class="fas fa-fw fa-atlas"></i> Atlas klimatické změny</a>
        <a href="/temata/emise/" class="btn btn-secondary"><i class="fas fa-fw fa-binoculars"></i> Explainery</a>
        <br/>
        <a href="/slovnik" class="btn btn-secondary"><i class="fas fa-fw fa-book"></i> Slovník pojmů</a>
        <a href="/jak-pouzivat" class="btn btn-secondary"><i class="fas fa-fw fa-book-reader"></i> Jak používat naše materiály</a>
      </div>
      <div class="col-md-6 col-lg-4">
        <a href="/atlas" class="card"><img src="/assets-local/img/atlas-mockup.png" alt="Alas klimatické změny" class="img-fluid"></a>
      </div>
    </div>
  </div></div>

  <div class="section tab-pane fade bg-extralight-red pt-4 pb-4" id="journalists" role="tabpanel" aria-labelledby="tab-role-journalists"><div class="container">
    <p class="lead">Pokud připravujete článek či se chystáte na diskusi nebo rozhovor, naše materiály vám pomohou získat přehled a aktuální data. I těžko srozumitelné problémy můžete díky našim grafikám prezentovat přehledně a srozumitelně. Data čerpáme z ověřených a transparentních zdrojů, posouzení jejich faktické správnosti jsme udělali za vás.</p>
    <p class="lead">Naše data a grafiky lze snadno sdílet, upravovat a šířit. Pokud je plánujete využít, nezapomeňte se prosím seznámit s pravidly jak používat naše materiály. Máte-li zájem o bližší informace o projektu nebo o spolupráci, kdykoli nás také můžete <a href="/jak-pouzivat#kontakt">kontaktovat</a>.</p>
    <a href="/jak-pouzivat" class="btn btn-primary"><i class="fas fa-fw fa-book-reader"></i> Jak používat naše materiály</a>
    <a href="/temata/emise/" class="btn btn-secondary"><i class="fas fa-fw fa-binoculars"></i> Explainery</a>
    <a href="/slovnik" class="btn btn-secondary"><i class="fas fa-fw fa-book"></i> Slovník pojmů</a>
  </div></div>
</div>

<div class="section section-new"><div class="container" markdown="1">

{:#new .display-2}
## Nejnovější materiály

{:.lead}
Zajímají vás naše novinky? V této sekci vždy najdete naše nejnovější infografiky, výtahy studií a datasety. Úplný seznam novinek a aktualit najdete i v [přehledu na samostatné stránce](/aktuality).

{% assign objects = site.infographics | concat: site.studies | concat: site.datasets | concat: site.explainers | sort: "published" | reverse %}
{% include preview-blocks.html blocks=objects link="news" limit=6 %}

</div></div>

{% assign sorted_index_tags = site.data.tags | where_exp: "item", "item.index-weight > 0" | sort: "index-weight" %}
<div class="section"><div class="container" markdown="1">
{: .display-2}
## Oblasti, kterým se věnujeme

{:.lead}
Klimatická změna je složitý komplex vzájemně provázaných jevů. Data, která sbíráme, třídíme a zpracováváme, se proto dotýkají různých oborů lidské činnosti – od ekonomiky přes politiku až po energetiku. Pro usnadnění orientace na webu třídíme naše materiály do níže uvedených kategorií.

<div class="accordion" id="accordionExample">
{% for index_tag in sorted_index_tags %}
<div class="accordion-item">
    <div class="accordion-header collapsed" id="heading_{{ index_tag.id }}" role="button" data-toggle="collapse" data-target="#collapse_{{ index_tag.id }}" aria-expanded="false" aria-controls="collapse_{{ index_tag.id }}">
        <h3 class="display-3">
        <span class="fa fa-fw fa-chevron-up"></span>
        {{ index_tag.name-long | capitalize }}
        <small class="text-secondary d-none d-md-inline">({% include includes-local/object-stats.html tag=index_tag.id %})</small>
        </h3>
    </div>
    <div class="collapse" id="collapse_{{ index_tag.id }}"  aria-labelledby="heading_{{ index_tag.id }}" data-parent="#accordionExample" markdown="1">
{:.lead}
{{ index_tag.description | markdownify }}

{% assign objects = site.infographics | concat: site.studies | concat: site.explainers | where_exp: "item", "item.tags contains index_tag.id" | sort: "weight" %}
{% include preview-blocks.html blocks=objects link=index_tag limit=6 %}

</div>
</div>
{% endfor %}
</div> <!-- accordion end -->

</div></div>
<div class="section"><div class="container clearfix" markdown="1">
{:#o-projektu .display-2}
## O nás a naší práci

{:.lead}
Projekt Fakta o klimatu usiluje o zkvalitnění společenské diskuse o klimatické změně.
Snažíme se dodávat srozumitelné údaje široké veřejnosti a vizuálně zpracovávat vědecké informace, aby bylo rozhodování ve věcech týkajících se klimatu založené na aktuálních a ověřených datech.

<div id="carousel_successes" class="carousel slide mb-4 mt-4" data-ride="carousel">
  <ol class="carousel-indicators">
    {%- assign filtered_success = site.data.carousel | where_exp: "item", "item.display != false" -%}
    {%- for item in filtered_success %}
    <li data-target="#carousel_successes" data-slide-to="{{- forloop.index0 -}}"{%- if forloop.index0 == 0 %} class="active"{%- endif -%}> </li>
    {%- endfor %}
  </ol>
  <div class="carousel-inner">
    {%- for item in filtered_success -%}
    {%- if item.link %}
    <a href="{{ item.link }}" {% if item.newtab %} target="_blank" {% endif %} class="no-ext-link-icon carousel-item {%- if forloop.index0 == 0 %} active{% endif %}" data-interval="6000">
    {%- else %}
    <div class="carousel-item {%- if forloop.index0 == 0 %} active{% endif %}" data-interval="6000">
    {%- endif %}
      <img src="/assets-local/carousel/{{ item.img }}" class="d-block w-100" alt="{{- item.title -}}" />
      <div class="carousel-caption d-none d-md-block">
        <h5>{{ item.title }}</h5>
        <p>{{ item.summary }}</p>
      </div>
    {%- if item.link %}
    </a>
    {%- else %}
    </div>
    {%- endif %}
    {%- endfor %}
  </div>
  <a class="carousel-control-prev" href="#carousel_successes" role="button" data-slide="prev">
    <span class="fas fa-chevron-left fa-3x" aria-hidden="true"></span>
    <span class="sr-only">Previous</span>
  </a>
  <a class="carousel-control-next" href="#carousel_successes" role="button" data-slide="next">
    <span class="fas fa-chevron-right fa-3x" aria-hidden="true"></span>
    <span class="sr-only">Next</span>
  </a>
</div>

{:.lead}
Debata o klimatické změně je komplikovaná a na všech stranách plná zbytečných emocí, polopravd a mýtů. Chceme poutat pozornost na důležitá témata a stavět most mezi vědci a lidmi, kterých se změny klimatu týkají. A to jsou všichni lidé.

{:.lead}
Jsme tým profesionálů zabývajících se různými obory – přírodovědou, informatikou, pedagogikou nebo komunikací. Pracuje na dobrovolnické bázi a finance na provoz získáváme od dárců, nepracujeme na ničí objednávku. Při naší činnosti komunikujeme s politiky, energetickými firmami i aktivistickými hnutími. Fakta o klimatu jsou však nezávislý projekt, který může podpořit každý.

<div class="row">
  <a href="/o-nas" class="btn btn-primary btn-lg col"><i class="fas fa-fw fa-info"></i> Více o projektu</a>
  <a href="{{ site.fundraising }}" class="btn btn-primary btn-lg col"><i class="fas fa-fw fa-heart"></i> Podpořte nás</a>
</div>

<a href="https://www.climate-kic.org/" class="no-ext-link-icon"><img class="index-logos float-right" src="/assets-local/img/logo-climate-kic.png" alt="Climate-KIC logo"/></a>
<a href="https://climatechallenge.impacthub.cz/" class="no-ext-link-icon"><img class="index-logos float-right" src="/assets-local/img/logo-climate-challenge.png" alt="Climate Challenge logo"/></a>

{:.lead}
V roce 2020 jsme zvítězili v akceleračním programu [Climate Challenge](https://climatechallenge.impacthub.cz/) pořádaným sítí podnikatelských inkubátorů [Impact Hub](https://impacthub.cz). V rámci toho náš projekt podpořila evropská iniciativa [Climate-KIC](https://www.climate-kic.org/), která hledá inovativní řešení na klimatickou krizi.

</div></div>
