# Шпаргалка по HTML и CSS для контент-менеджера

1. [Форматирование текста](#1-Форматирование-текста)
2. [Создание таблицы](#2-Создание-таблицы)
3. [Добавление стилей](#3-Добавление-стилей)

## 1. Форматирование текста

<table>
  <thead>
    <th>Мне надо:</th>
    <th>Нужно писать:</th>
    <th>Выглядеть будет:</th>
  </thead>
  <tbody>
    <tr>
      <td>Вставить параграф</td>
      <td><code><p>Текст параграфа</p></code>
      </td>
      <td><p>Первый параграф</p><p>Второй параграф</p></td>
    </tr>
    <tr>
      <td>Перенести текст на строку ниже</td>
      <td><code>Текст ниже будет с новой строки<br></code></td>
      <td>В отличие от тега p,<br> тег br не создает пустую строку</td>
    </tr>
    <tr>
      <td>Разместить заголовок</td>
      <td><code><h5>Существует шесть уровней заголовков: от h1 до h6</h5></code></td>
      <td><h5>На странице должен быть только один заголовок первого уровня</h5></td>
    </tr>
    <tr>
      <td>Добавить цитату</td>
      <td>
        <code>
          <blockquote>
          Я помню чудное мгновенье!
          </blockquote>
        </code>
      </td>
      <td>
        <blockquote>
        Я помню чудное мгновенье!
        </blockquote>
      </td>
    </tr>
    <tr>
      <td>Выделить текст жирным</td>
      <td><code><b>Я - жирный текст</b></code></td>
      <td><b>Визуально, текст идентичен важному.</b></td>
    </tr>
    <tr>
      <td>Выделить важный текст</td>
      <td><code><strong>Я – важный текст!</strong></code></td>
      <td><strong>Но смысл разный.</strong></td>
    </tr>
    <tr>
      <td>Выделить текст курсивом</td>
      <td><code><i>Я написан курсивом</i></code></td>
      <td><i>Тоже самое с курсивом</i></td>
    </tr>
    <tr>
      <td>Сделать смысловой акцент</td>
      <td><code><em>Смысловой акцент</em></code></td>
      <td><em>Визуально одиноково, а смысл разный</em></td>
    </tr>
    <tr>
      <td>Вставить ссылку</td>
      <td><code><a href="http://netology.ru/">Нетология</a></code></td>
      <td><a href="http://netology.ru">Кликать сюда</a></td>
    </tr>
    <tr>
    <td>Вставить картинку</td>
      <td><code><img src="img/no-foto.jpg" alt="картинка"></code></td>
      <td><img src="../../img/no-photo.png" alt="Нет фото"></td>
    </tr>
    <tr>
      <td>Логически связать картинку и подпись</td>
      <td>
        <pre>
          <code>
            <figure>
                <img src="images/no-photo.png" alt="Нет фото">
                <figcaption>Нет фото</figcaption>
              </figure>
          </code>  
        </pre>
      </td>
      <td>
        <figure>
          <img src="../../img/no-photo.png" alt="Нет фото">
          <figcaption>Нет фото</figcaption>
        </figure>
      </td>
    </tr>
    <tr>
      <td>Задать класс тегу</td>
      <td>
        <code><p class="new">Абзац с классом</p></code>
      </td>
      <td>В CSS это выглядит вот <a href="#new">так</a></td>
    </tr>
    <tr>
      <td>Задать идентификатор тегу</td>
      <td><code><p id="unique">Абзац с идентификатором</p></code></td>
      <td>В CSS это выглядит вот <a href="#unique">так</a></td>
    </tr>
    <tr>
      <td>Создать маркированный список</td>
      <td>
        <pre>
          <code>
            <ul>
              <li>Певый пункт</li>
              <li>Второй пункт</li>
              <li>Третий пункт</li>
            </ul>
          </code>
        </pre>   
      </td>
      <td>
        <ul>
          <li>Первый пункт</li>
          <li>Второй пункт</li>
          <li>Третий пункт</li>
        </ul>
      </td>    
   </tr>
        <tr>
      <td>Создать нумерованный список</td>
      <td>
        <pre>
          <code>
            <ol>
              <li>Певый пункт</li>
              <li>Второй пункт</li>
              <li>Третий пункт</li>
            </ol>
          </code>
        </pre>   
      </td>
      <td>
        <ol>
          <li>Первый пункт</li>
          <li>Второй пункт</li>
          <li>Третий пункт</li>
        </ol>
      </td>    
   </tr>
    <tr>
      <td>Изменить нумерацию в списке</td>
      <td>
        <pre>
          <code>
            <ol start="3">
            ...
            </ol>
          </code>
        </pre>
      </td>
      <td>
        <ol start="3">
          <li>Три</li>
          <li>Четыре</li>
          <li>Пять</li>
        </ol>     
      </td>
    </tr>
    <tr>
      <td>Создать список определений</td>
      <td>
        <pre>
          <code>
            <dl>
              <dt>Первое определение</dt>
              <dd>Расшифровка первого определения</dd>
              <dt>Второе определение</dt>
              <dd>Расшифровка второго определения</dd>
            </dl>
          </code>
        </pre>
      </td>
      <td>
        <dl>
          <dt>Первое определение</dt>
          <dd>Расшифровка первого определения</dd>
          <dt>Второе определение</dt>
          <dd>Расшифровка второго определения</dd>
        </dl>
      </td>
    </tr>    
    <tr>
      <td>Вложить один список в другой</td>
        <td>
          <pre>
            <code>
              <ol>
                <li>Пункт списка
                  <ul>
                    <li>Пункт вложенного списка</li>
                  </ul>
                </li>
              </ol>
            </code>
          </pre>
        </td>
        <td>
          <ol>
            <li> Пункт списка
            <ul>
              <li>Пункт вложенного списка</li>
            </ul>
          </li>
        </ol>
      </td>
    </tr>  
  </tbody>
</table>


  </section>
  <section class="chapter-table">
    <h2 id="table">Создание таблицы</h2>
    <code>&lt;table&gt;</code>
    <table>
      <caption>&lt;caption&gt;Таблица 1. Как правильно сверстать таблицу&lt;/caption&gt;</code></caption>
      <thead>
        <tr>
          <th class="no-border"><code>&lt;thead&gt;&lt;tr&gt;</code></th>
          <th><code>&lt;th&gt;...&lt;/th&gt;</code></th>
          <th><code>&lt;th&gt;...&lt;/th&gt;</code></th>
          <th><code>&lt;th&gt;...&lt;/th&gt;</code></th>
          <th><code>&lt;th&gt;...&lt;/th&gt;</code></th>
          <th><code>&lt;th&gt;...&lt;/th&gt;</code></th>
          <th class="no-border"><code>&lt;/tr&gt;&lt;/thead&gt;</code></th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td class="no-border"><code>&lt;tbody&gt;&lt;tr&gt;</code></td>
          <td rowspan="2"><code>&lt;td rowspan="2"&gt;<br>...<br>&lt;/td&gt;</code></td>
          <td colspan="2"><code>&lt;td colspan="2"&gt;...&lt;/td&gt;</code></td>
          <td ><code>&lt;td&gt;...&lt;/td&gt;</code></td>
          <td><code>&lt;td&gt;...&lt;/td&gt;</code></td>
          <td class="no-border"><code>&lt;/tr&gt;</code></td>
        </tr>
        <tr>
          <td class="no-border"><code>&lt;tr&gt;</code></td>
          <td colspan="3" rowspan="3"><code>&lt;td colspan="3" rowspan="3"&gt;<br>...<br>&lt;/td&gt;</code></td>
          <td><code>&lt;td&gt;...&lt;/td&gt;</code></td>
          <td class="no-border"><code>&lt;/tr&gt;</code></td>
        </tr>
        <tr>
          <td class="no-border"><code>&lt;tr&gt;</code></td>
          <td><code>&lt;td&gt;...&lt;/td&gt;</code></td>
          <td><code>&lt;td&gt;...&lt;/td&gt;</code></td>
          <td class="no-border"><code>&lt;/tr&gt;</code></td>
        </tr>
        <tr>
          <td class="no-border"><code>&lt;tr&gt;</code></td>
          <td><code>&lt;td&gt;...&lt;/td&gt;</code></td>
          <td><code>&lt;td&gt;...&lt;/td&gt;</code></td>
          <td class="no-border"><code>&lt;/tr&gt;&lt;/tbody&gt;</code></td>
        </tr>
      </tbody>
      <tfoot>
        <tr>
          <td class="no-border"><code>&lt;tfoot&gt;&lt;tr&gt;</code></td>
          <td><code>&lt;td&gt;...&lt;/td&gt;</code></td>
          <td><code>&lt;td&gt;...&lt;/td&gt;</code></td>
          <td><code>&lt;td&gt;...&lt;/td&gt;</code></td>
          <td><code>&lt;td&gt;...&lt;/td&gt;</code></td>
          <td><code>&lt;td&gt;...&lt;/td&gt;</code></td>
          <td class="no-border"><code>&lt;/tr&gt;&lt;/tfoot&gt;</code></td>
        </tr>
      </tfoot>
    </table>
    <code>&lt;/table&gt;</code>
  </section>
  <section class="chapter-css">
    <h2 id="css">Добавление стилей</h2>
    <table>
      <thead>
        <th>Селектором может быть:</th>
        <th>Запишем как:</th>
      </thead>
      <tbody>
        <tr>
          <td>Тег</td>
          <td>p {...};</td>
        </tr>
        <tr>
          <td>Класс</td>
          <td id="new">.new {...};</td>
        </tr>
        <tr>
          <td>ID</td>
          <td id="unique">#unique {...}</td>
        </tr>
      </tbody>
    </table>
    <table>
      <caption class="table-css">Основные свойства стилей</caption>
      <thead>
        <th>Хочу изменить:</th>
        <th>Свойства</th>
        <th>Что получаем</th>
      </thead>
      <tbody>
        <tr>
          <td rowspan="4">Текст</td>
          <td>
            <script type="text/plain" class="language-markup language-css">
            p {
              font-size: 20px;
            }
            </script>
          </td>
          <td style="font-size:20px">Текст на 20px</td>
        </tr>
        <tr>
          <td>
            <script type="text/plain" class="language-markup language-css">
            p {
              font-weight: 700;
            }
            </script>
          </td>
          <td style="font-weight:700">Жирный текст</td>
        </tr>
        <tr>
          <td>
            <script type="text/plain" class="language-markup language-css">
            p {
              font-style: italic;
            }
            </script>
          </td>
          <td style="font-style:italic">Наклонный текст</td>
        </tr>
        <tr>
          <td>
            <script type="text/plain" class="language-markup language-css">
            p {
              color: red;
            }
            </script>
          </td>
          <td style="color:red">Красный текст</td>
        </tr>
        <tr>
          <td>Маркированный список</td>
          <td>
            <script type="text/plain" class="language-markup language-css">
            ul {
              list-style-type: disc;
            }
            </script>
          </td>
          <td>
            <ul style="list-style-type: disc">
              <li>disc</li>
            </ul>
            <ul style="list-style-type: circle">
              <li>circle</li>
            </ul>
            <ul style="list-style-type: square">
              <li>square</li>
            </ul>
          </td>
        </tr>
        <tr>
          <td>Нумерованный список</td>
          <td>
            <script type="text/plain" class="language-markup language-css">
            ol {
              list-style-type: decimal;
            }
            </script>
          </td>
          <td>
            <ol style="list-style-type: decimal">
              <li>decimal</li>
            </ol>
            <ol style="list-style-type: lower-roman" start="2">
              <li>lower-roman</li>
            </ol>
            <ol style="list-style-type: upper-roman" start="3">
              <li>upper-roman</li>
            </ol>
            <ol style="list-style-type: lower-alpha" start="4">
              <li>lower-alpha</li>
            </ol>
            <ol style="list-style-type: upper-alpha" start="5">
              <li>upper-alpha</li>
            </ol>
          </td>
        </tr>
        <tr>
          <td rowspan="2">Фон</td>
          <td>
            <script type="text/plain" class="language-markup language-css">
            div {
              background-color: lightblue;
            }
            </script>
          </td>
          <td style="background-color: lightblue">Светло-синий фон</td>
        </tr>
        <tr>
          <td>
            <script type="text/plain" class="language-markup language-css">
            div {
              background-image: url(images/no-photo.png);
            }
            </script>
          </td>
          <td style="background-image:url(../../img/no-photo.png); background-size: contain; background-repeat: no-repeat; height: 150px; vertical-alighn:bottom;">Фоновое изображение</td>
        </tr>
      </tbody>
    </table>
  </section>
</main>
<script src="../../js/prism.js"></script>
<script src="../../js/scroll.js"></script>
<script src="https://unpkg.com/social-likes-next/dist/social-likes.min.js"></script>
</body>
</html>
