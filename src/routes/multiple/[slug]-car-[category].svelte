<script context="module">
    export async function preload({params,query}){
        let data = params;
        console.log(params)
        return {data};
    }
</script>


<script>
 export let data;
</script>

This is a page that contains data of {data.slug} and {data.category}




<img src="https://media.giphy.com/media/qqD2dzGdJTmda/giphy.gif" alt="{data.slug} and {data.category}">


<style>
    img {
        display: flex;
        margin: 0 auto;
        padding-top:2em;
    }
</style>


