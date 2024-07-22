<script>
    export let text = null;
    export let pixels = 15;
    export let bold = false;
    export let style = null;
</script>

<div>
    <p style="font-size: {pixels}px; {bold ? "font-weight:bold" : ""}; {style}">{text}<slot/></p>
</div>


<style>
    p {
        margin: auto;
    }
</style>