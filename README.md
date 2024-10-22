<h1 align="center">Escaped 🏃🏻‍♂️‍➡️ for Astro 🚀</h1>

<br>

<div align="center">
  🏃🏻‍♂️‍➡️ An Astro component that holds only HTML-encoded content. 📜
</div>

<br>
<br>

<div align="center">
  <blockquote>
    <br>
    <h4>💖 Support further development</h4>
    <span>I work hard for every project, including this one
    <br>
    and your support means a lot to me!
    <br>
    <br>
    Consider buying me a coffee. ☕
    <br>
    <strong>Thank you for supporting my efforts! 🙏😊</strong></span>
    <br>
    <br>
    <a href="https://ko-fi.com/igorskyflyer" target="_blank"><img src="https://raw.githubusercontent.com/igorskyflyer/igorskyflyer/main/assets/ko-fi.png" alt="Donate to igorskyflyer" width="150"></a>
    <br>
    <br>
    <a href="https://github.com/igorskyflyer"><em>@igorskyflyer</em></a>
    <br>
    <br>
    <br>
  </blockquote>
</div>

<br>
<br>

## 📃 Table of contents

- [Usage](#-usage)
- [API](#-api)
- [Examples](#-examples)
- [Changelog](#-changelog)
- [License](#-license)
- [Related](#-related)
- [Author](#-author)

<br>
<br>

## 🕵🏼 Usage

Install it by executing:

```shell
npm i -D "@igor.dvlpr/astro-escaped-component"
```

<br>

## 🤹🏼 API

The API exposes a single Astro component `Escaped`, see [a usage example below](#-examples).  

After importing the component into a project, add it to an `Astro` page markup as:

```astro
<Escaped is:raw>
 {/* text/code to be escaped */}
</Escaped>
```

<br>

> [!IMPORTANT]
> The attribute `is:raw` is crucial for the component to work, if not specified, Astro will parse all content as pure HTML, including `<script>` and `<style>` tags.
>

<br>

> [!CAUTION]
> This component escapes/encodes text using HTML entities and can help prevent XSS attacks. However, this may not be ***sufficient*** in all cases.
>
> Ensure **additional** security measures are in place.
>

<br>

---

## ✨ Examples

`example.astro`
```astro
---
import Escaped from '@igor.dvlpr/astro-escaped-component'
---

<Escaped is:raw>
  Mitochondria are known as the "powerhouses" of the cell because they generate most of the cell's supply of ATP & CO<sub>2</sub>, which is used as a source of chemical energy.
  
  <, >, ", ', &, =, `, !, @, $, %, (, ), +, {, }, [, ].
  
  <script>console.log('Hello? No? 😭')</script>
</Escaped>

{/*

  Will be rendered as:

  Mitochondria are known as the &#34;powerhouses&#34; of the cell because they generate most of the cell&#39;s supply of ATP &#38; CO&#60;sub&#62;2&#60;/sub&#62;, which is used as a source of chemical energy.

  &#60;, &#62;, &#34;, &#39;, &#38;, &#61;, &#96;, &#33;, &#64;, &#36;, &#37;, &#40;, &#41;, &#43;, &#123;, &#125;, &#91;, &#93;.

  &#60;script&#62;console.log&#40;&#39;Hello? No? 😭&#39;&#41;&#60;/script&#62;

*/}
```

---

## 📝 Changelog

📑 The changelog is available here: [CHANGELOG.md](https://github.com/igorskyflyer/npm-astro-escaped-component/blob/main/CHANGELOG.md).

---

## 🪪 License

Licensed under the MIT license which is available here, [MIT license](https://github.com/igorskyflyer/npm-astro-escaped-component/blob/main/LICENSE).

---

## 🧬 Related

[@igor.dvlpr/common-types](https://www.npmjs.com/package/@igor.dvlpr/common-types)

> _🔦 Provides frequently used types for your TypeScript projects. 🦄_

<br>

[@igor.dvlpr/registry-apppaths](https://www.npmjs.com/package/@igor.dvlpr/registry-apppaths)

> _🪀 A Node.js module for reading the AppPaths registry key on Windows. Useful for retrieving applications that can be launched from the command prompt. 🗃_

<br>

[@igor.dvlpr/scrollend-polyfill](https://www.npmjs.com/package/@igor.dvlpr/scrollend-polyfill)

> _🛴 A performant and light (< 1.5KB) JavaScript polyfill for the scrollend Event. ⛸️_

<br>

[@igor.dvlpr/astro-easynav-button](https://www.npmjs.com/package/@igor.dvlpr/astro-easynav-button)

> _🧭 Add an easy-to-use navigational button (jump to top/bottom) to your Astro site. 🔼_

<br>

[@igor.dvlpr/windev](https://www.npmjs.com/package/@igor.dvlpr/windev)

> _🍃 Provides ways of checking whether a path is a legacy Windows device. 💾_

---

<br>

### 👨🏻‍💻 Author
Created by **Igor Dimitrijević** ([*@igorskyflyer*](https://github.com/igorskyflyer/)).
