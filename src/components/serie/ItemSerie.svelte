<script lang="ts">
    export let serie: any = null;
</script>

{#if serie}
    <a href="/serie/{serie.id}" class="flex flex-col rounded-md overflow-hidden border border-zinc-800">
       <img src = {serie.imagem} alt="Imagem da Serie" class="h-96 object-cover" />
    </a>
    <div class="flex flex-col gap-2 p-5">
        <span class="text-2x1 font-black">{serie.titulo}</span>
        <span class="text-sm text-zinc-400 text-justify">{serie.descricao}</span>
        <button>Leia Mais</button>
    </div>
{/if}