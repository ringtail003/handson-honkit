{% import "../parts/notice.html" as noticeIcon %}
{% import "../icons/chevron-right.html" as chevronRightIcon %}

<nav class="flex gap-4 items-center text-sm breadcrumbs">
  {%- block breadcrumbs %}
    <a href="/">トップ</a>
    <div class="h-8 w-8 text-gray-400">{{- chevronRightIcon.render() }}</div>
    <a href="/chapter1/1-1.html">セットアップ</a>
    <div class="h-8 w-8 text-gray-400">{{- chevronRightIcon.render() }}</div>
  {%- endblock %}
</nav>

<h1 class="text-2xl font-bold">
  {% block title %}{% endblock %}
</h1>

{% block contents %}
{% endblock %}

<hr>

<div class="my-14">
  <div class="text-xl font-bold mb-4">もっと知りたい</div>
  <div class="grid grid-cols-2 gap-8">
    {{- noticeIcon.render("新着情報", "最近の投稿をチェックしたい") }}
    {{- noticeIcon.render("活用ガイド", "活用方法や関連情報を知りたい") }}
  </div>
</div>
