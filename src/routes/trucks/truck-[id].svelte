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

Your imaginary logistics service that contains data of truck id: <code>{data.id}</code> and the url is trucks/trucks-{data.id}



<img src="https://media.giphy.com/media/FqtWrearu5vb2/giphy.gif" alt="{data.id}">


<style>
    img {
        display: flex;
        margin: 0 auto;
        padding-top:2em;
    }
</style>