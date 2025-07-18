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
    <h1 class="text-4xl pb-1 pt-2 text-blue-600">{@html autor.nome}</h1>
    <article class="prose lg:prose-xl prose-invert text-justify text-blue-200">
      {@html autor.apresentacao}
    </article>

    <h1 class="text-4xl pb-1 pt-2 text-blue-600">{@html autor.destaque02}</h1>
    <article class="prose lg:prose-xl prose-invert text-justify text-blue-200">
      {@html autor.texto02}
    </article>

    <h1 class="text-4xl pb-1 pt-2 text-blue-600">{@html autor.destaque03}</h1>
    <article class="prose lg:prose-xl prose-invert text-justify text-blue-200">
      {@html autor.texto03}
      <br />
      <ul  class="pl-5 italic text-blue-400">
        {#each autor.obra as item}
          <li>{@html item}</li>
        {/each}
      </ul>
    </article>

    <h1 class="text-4xl pb-1 pt-2 text-blue-600">{@html autor.destaque04}</h1>
    <article class="prose lg:prose-xl prose-invert text-justify text-blue-200">
      {@html autor.texto04}
    </article>

    <h1 class="text-4xl pb-1 pt-2 text-blue-600">{@html autor.destaque05}</h1>
    <article class="prose lg:prose-xl prose-invert text-justify text-blue-200">
      {@html autor.texto05}
    </article>

    <h1 class="text-4xl pb-1 pt-2 text-blue-600">{@html autor.destaque06}</h1>
    <article class="prose lg:prose-xl prose-invert text-justify text-blue-200">
      {@html autor.texto06}
    </article>

    <hr />

    <article class="prose lg:prose-xl prose-invert text-justify talic text-blue-500">
      {@html autor.citacao}
    </article>
  </div>
{/if}
