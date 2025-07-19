<script lang="ts">
    import { marked } from "marked";

    export let autor: any = null;
</script>

{#if autor}
    <div class="flex flex-col gap-5">
        <img
            src={autor.imagem}
            alt="Foto do autor"
            class="h96 object-cover rounded-md"
        />

        <article>
            <h1 class="text-4xl pb-1 pt-2 text-blue-600">{@html autor.nome}</h1>

            <div class="prose lg:prose-xl prose-invert text-justify text-blue-200"           >
                {@html autor.apresentacao}
            </div>

            <h1 class="text-4xl pb-1 pt-2 text-blue-600">
                {@html autor.destaque02}
            </h1>

            <div class="prose lg:prose-xl prose-invert text-justify text-blue-200">
                {@html autor.texto02}
            </div>

            <h1 class="text-4xl pb-1 pt-2 text-blue-600">
                {@html autor.destaque03}
            </h1>

            <div class="prose lg:prose-xl prose-invert text-justify text-blue-200">
                {@html autor.texto03}
                <br />
                <ul class="pl-5 italic text-blue-400">
                    {#each autor.obra as item}
                        <li>{@html item}</li>
                    {/each}
                </ul>
            {#if autor.texto03b}    
                <div class="prose lg:prose-xl prose-invert text-justify pt-5 text-blue-200">
                    {@html autor.texto03b}
                </div>
            {/if}

            </div>

            <h1 class="text-4xl pb-1 pt-2 text-blue-600">
                {@html autor.destaque04}
            </h1>

            <div class="prose lg:prose-xl prose-invert text-justify text-blue-200">
                {@html autor.texto04}
            </div>

            <h1 class="text-4xl pb-1 pt-2 text-blue-600">
                {@html autor.destaque05}
            </h1>

            <div class="prose lg:prose-xl prose-invert text-justify text-blue-200">
                {@html autor.texto05}
            </div>

                        <h1 class="text-4xl pb-1 pt-2 text-blue-600">
                {@html autor.destaque06}
            </h1>

            <div class="prose lg:prose-xl prose-invert text-justify text-blue-200">
                {@html autor.texto06}
            </div>
            <br>
            <br>
            <hr />
            <br>
            <div class="prose lg:prose-xl prose-invert text-center text-lg truncate talic text-blue-500">
                {@html autor.citacao}
            </div>
        </article>
    </div>
{/if}
