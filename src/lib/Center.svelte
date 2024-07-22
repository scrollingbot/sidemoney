<script>
    export let height=0;
    export let color = null;
    export let style = null;
</script>

<div class="center-widget" style="background-color: {color}; {height>0 ? "height:"+{height}+"vh;": "height:inherit;"} {style}">
    <slot/>
</div>


<style>
    .center-widget {
        overflow: auto;
        display: flex;
        align-items: center;
        justify-content: center;
        text-align: center;
        height: 100vh;
    }
</style>