<script lang="ts">
    export let valor: string;
    $: tamanhoFonte = valor.length > 20 ? "pequena" : `s-${valor.length}`;
</script>

<div class={`tela ${tamanhoFonte}`}>
    <span>{valor}</span>
</div>

<style>
    .tela {
        display: flex;
        justify-content: flex-end;
        align-items: center;
        background-color: white;
        flex: 1;
        padding: 0px 5px;
        overflow: hidden;
        font-size: 1.7em;
        margin: 1px;
        border-top-right-radius: 5px;
        border-top-left-radius: 5px;
    }

    .s-10 {
        font-size: 1.5em;
    }
    .s-11 {
        font-size: 1.35em;
    }
    .s-12 {
        font-size: 1.25em;
    }
    .s-13 {
        font-size: 1.18em;
    }
    .s-14 {
        font-size: 1.1em;
    }
    .s-15 {
        font-size: 1em;
    }
    .s-16 {
        font-size: 0.95em;
    }
    .s-17 {
        font-size: 0.9em;
    }
    .s-18 {
        font-size: 0.85em;
    }
    .s-19 {
        font-size: 0.8em;
    }
    .s-20 {
        font-size: 0.75em;
    }
    .pequena {
        font-size: 0.6em;
    }
</style>
