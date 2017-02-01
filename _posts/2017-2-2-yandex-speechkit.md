---
layout: post
title: Speech
---

<script src="https://webasr.yandex.net/jsapi/v1/webspeechkit.js" type="text/javascript"></script>

https://tech.yandex.ru/speechkit/jsapi/doc/dg/concepts/settings-docpage/
<div id="my_id" style="width: 200px"></div>

<script>
window.onload = function () {
// Задаем глобальные настройки API.
// Язык речи.
window.ya.speechkit.settings.lang = 'ru-RU';
// API-ключ.
// window.ya.speechkit.settings.apikey = 'aqVfh3r8...';

  var textline = new ya.speechkit.Textline('my_id', {
        apikey: '66e87f44-022c-454a-baed-917e28d3d3ad',
        onInputFinished: function(text) {
          // Финальный текст.
          alert(text);
        }
      });
};
</script>
