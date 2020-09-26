<script context="module">
  export async function preload({ params, query }) {
    let parts = params;

    return { parts };
  }
</script>

<script>
    export let parts;

</script>

<h1>You are on the /posts/{parts.parts[0]}.</h1>
<ul>
  <li>
    Current location returns {JSON.stringify(parts)} 
  </li>
  <li>
    <a href="./posts/en/postname">Try going here to capture the slug</a>
  </li>

  <li>Refer <a href="https://sapper.svelte.dev/docs/#Pages">https://sapper.svelte.dev/docs/#Pages</a></li>

</ul>

<p>Directory Structure</p>

<pre>
    └───routes
    │   └───posts
    │       └───[...parts]
    |       |       └───
    │       │       [slug].svelte 
    │       │       index.svelte
    │       │ index.svelte
</pre>