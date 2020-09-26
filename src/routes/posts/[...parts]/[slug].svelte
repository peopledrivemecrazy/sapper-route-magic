
<script context="module">
  export async function preload({ params, query }) {
    console.log(params);
    let parts = params
    return {parts}
  }
</script>
<script>
    export let parts
    console.log(parts.parts.length)
</script>

<h1>You are on the /posts/{parts.parts.map(e=>e).join('/')}/{parts.slug}.</h1>
<ul>
  <li>
    You have captured the slug <code> {parts.slug}</code>
  </li>
  {#if (parts.parts.length < 2)}
  <li>
    <a href="/posts/en/category/postname">Since [...parts] are spread this can be drilled down to capture more <code>params</code></a>
  </li>
  {/if}
  <li>Refer <a href="https://sapper.svelte.dev/docs/#Pages">https://sapper.svelte.dev/docs/#Pages</a></li>

</ul>
