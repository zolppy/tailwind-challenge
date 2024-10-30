<div align="center">
  <h1>Desafio de Tailwind CSS: Página de Menu de Restaurante</h1>
  <p>Este projeto consiste da implementação de uma página web estática (não é necessário o uso de JavaScript) para prática e aperfeiçoamento de habilidades no uso do <em>framework</em> Tailwind CSS.</p>
</div>

<h2>Requisitos Mínimos</h2>
<ul>
  <li>A página deverá ser responsiva a dispositivos desktop e mobile;</li>
  <li>Dever-se-á fazer uso <strong>somente</strong> de Tailwind CSS, no tocante à estilização;</li>
  <li>O HTML deve ser semântico (uso de tags semânticas);</li>
  <li>A página deverá conter pelo menos duas seções, seção de pratos e seção de contato;</li>
  <li>O site deverá ser SPA (<em>Single Page Application</em>), ou seja, de uma única página;</li>
  <li>Deverá haver um cabeçalho (header) fixo, com links para cada seção descrita anteriormente, logo, nome do site e slogan;</li>
  <li>A seção de pratos deverá conter os tipos de pratos: entradas, pratos principais, sobremesas e bebidas, com pelo menos três itens em cada tipo;</li>
  <li>Rodapé (footer) com pelo menos o link para o repositório do projeto no GitHub;</li>
  <li>O código deverá estar organizado (identação, sem espaços em branco desnecessários, mais de uma quebra de linha consecutivas...)</li>
</ul>
<p>Obs.: não é necessário que o conteúdo da página, incluíndo imagens, seja real, poder-se-á utilizar "lorem ipsum" (conteúdo fictício, template), pois o foco maior está na interface.</p>

<h2>Como Importar Tailwind CSS a uma página HTML, via CDN (<em>Content Delivery Network</em>)</h2>
<pre><code><script src="https://cdn.tailwindcss.com"></script></code></pre>
<p>Ao colar o código acima ao <em>head</em> da página, já será possível utilizar o <em>framework</em>.</p>

<pre>
<code>
<script>
  tailwind.config = {
    theme: {
      extend: {},
    },
    corePlugins: {
      preflight: true,
    },
  }
</script>
</code>
</pre>
<p>Esse segundo código é opcional, porém é fortemente aconselhável utilizá-lo, pois traz alguns benefícios a mais do <em>framework</em>, como o <em>reset</em> de estilos padrão, que podem variar em diferentes navegadores, por exemplo.</p>

<h2>Como Utilizar Tailwind CSS</h2>
<p>Com a tecnologia devidamente importada, bastará utilizar classes específicas a elementos HTML, de acordo com o que se desejar fazer, por exemplo:</p>
<pre><code>&lt;div class="flex flex-col flex-wrap">&lt;/div></code></pre>

<p>Produzirá exatamente o mesmo efeito que:</p>
<pre>
  <code>
    div {
      display: flex;
      flex-direction: column;
      flex-wrap: wrap;
    }
  </code>
</pre>
