<script>
    export let width = 100;
    export let height = 100;
    export let color = null;
    export let style = null;
</script>

<div class="container-widget" style="background-color: {color}; width: {width}%; height: {height}vh; {style}">
    <slot/>
</div>

