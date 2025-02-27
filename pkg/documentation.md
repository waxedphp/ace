# Ace

Ace is an embeddable code editor written in JavaScript.
It matches the features and performance of native editors such as Sublime, Vim and TextMate.
It can be easily embedded in any web page and JavaScript application.
Ace is maintained as the primary editor for Cloud9 IDE and is the successor of the Mozilla Skywriter (Bespin) project.

https://ace.c9.io/

Other license

---

### PHP:

```php
  use Waxedphp\Ace\Setter as Ace;
  
  $obj = new Ace($this->waxed);
  
  $obj->setMode('pascal');
  $obj->setTheme('dracula');

  $this->waxed->pick('section1')->display([
    'data' => [
      'payload' => $obj->value("program Test;\nuses MyLib;\nbegin\n  writeln('Hello world.');\nend.\n"),
  ]],$this->tpl.'/ace');

```

---
### HTML:

```html

<textarea class="waxed-ace"
  name="code"
  style="height:200px;"
  data-name="data.payload" >

</textarea>

```
---
---

### PHP methods:

```php

  use Waxedphp\Ace\Setter as Ace;
  
  $obj = new Ace($this->waxed);
  
  // sets the language
  $obj->setMode('pascal');
  
  // sets the theme
  $obj->setTheme('dracula');

  // sets the content of editor and returns settings to frontend
  $obj->value("program Test;\nuses MyLib;\nbegin\n  writeln('Hello world.');\nend.\n");

```



### License:

```
Copyright (c) 2010, Ajax.org B.V.
All rights reserved.

Redistribution and use in source and binary forms, with or without
modification, are permitted provided that the following conditions are met:
    * Redistributions of source code must retain the above copyright
      notice, this list of conditions and the following disclaimer.
    * Redistributions in binary form must reproduce the above copyright
      notice, this list of conditions and the following disclaimer in the
      documentation and/or other materials provided with the distribution.
    * Neither the name of Ajax.org B.V. nor the
      names of its contributors may be used to endorse or promote products
      derived from this software without specific prior written permission.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
DISCLAIMED. IN NO EVENT SHALL AJAX.ORG B.V. BE LIABLE FOR ANY
DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
(INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```
