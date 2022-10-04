{% import "../icons/chevron-right.html" as chevronRightIcon %}

<nav class="breadcrumbs">
  {%- block breadcrumbs %}
    <a href="/">トップ</a>
    <div class="icon">{{- chevronRightIcon.render() }}</div>
    <a href="/issue.html">詰まったところ</a>
    <div class="icon">{{- chevronRightIcon.render() }}</div>
  {%- endblock %}
</nav>

<div class="flex justify-between items-center">
  <h1 class="text-2xl font-bold flex-1">{{ page.title }}</h1>
  {% if page.updatedAt %}
    <span class="text-xs whitespace-nowrap">更新日：{{ page.updatedAt }}</span>
  {% endif %}
</div>

{% block contents %}
{% endblock %}
