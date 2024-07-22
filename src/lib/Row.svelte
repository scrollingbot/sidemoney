<script>
    export let width = 100;
    export let color = null;
    export let style = null;
    export let align = "space-evenly";
</script>

<div class="row-widget" style="background-color: {color}; width: {width}%;">
    <ul class="row" style="justify-content: {align};  {style}">
        <slot/>
    </ul>
</div>


<style>
    .row {
        display: flex;
        flex-wrap: wrap;
        list-style: none;
        margin: 0px;
        padding: 0;
    }
</style>