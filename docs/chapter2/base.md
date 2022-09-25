{% import "../parts/tag.html" as tag %}
{% import "../icons/chevron-right.html" as chevronRightIcon %}

<nav class="flex gap-4 items-center text-sm breadcrumbs">
  {%- block breadcrumbs %}
    <a href="/">トップ</a>
    <div class="h-8 w-8 text-gray-400">{{- chevronRightIcon.render() }}</div>
    <a href="/chapter2/2-1.html">使い方</a>
    <div class="h-8 w-8 text-gray-400">{{- chevronRightIcon.render() }}</div>
  {%- endblock %}
</nav>

<h1 class="text-2xl font-bold">
  {% block title %}{% endblock %}
</h1>

{% block contents %}
{% endblock %}

<hr>

{% block keywords %}
  <div class="my-14">
    <div class="text-lg font-bold mb-4">同じカテゴリの記事</div>
    <div class="flex gap-2">
      {% if page.search.keywords|length == 0 %}
      ありません
      {% endif %}
      {%- for keyword in page.search.keywords -%}
        {{- tag.render(keyword) -}}
      {%- endfor -%}
    </div>
  </div>
{% endblock %}
