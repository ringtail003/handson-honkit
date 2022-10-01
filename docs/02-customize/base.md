{% import "../icons/chevron-right.html" as chevronRightIcon %}

<nav class="breadcrumbs">
  {%- block breadcrumbs %}
    <a href="/">トップ</a>
    <div class="icon">{{- chevronRightIcon.render() }}</div>
    <a href="/02-customize/2-1.html">使い方</a>
    <div class="icon">{{- chevronRightIcon.render() }}</div>
  {%- endblock %}
</nav>

<h1 class="text-2xl font-bold">
  {% block title %}{% endblock %}
</h1>

{% block contents %}
{% endblock %}
