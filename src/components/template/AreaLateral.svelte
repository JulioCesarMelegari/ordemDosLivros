<script>
    import Menu from "./Menu.svelte";
    import MenuItem from "./MenuItem.svelte";

</script>
<aside class="
    flex flex-col self-start
    border border-zinc-800 p-5 rounded-md
    gap-10 w-72"
>
    <Menu titulo="Navegação">
        <MenuItem texto="Início" href="/" />
        <MenuItem texto="Personagens" href="/" />
        <MenuItem texto="Autores" href="/" />
        <MenuItem texto="Séries" href="/" />
    </Menu>
    <Menu titulo="Principais Autores">
        <MenuItem texto="J.k. Rowling" href="/autores/j-k-rowling" />
        <MenuItem texto="J.R.R. Tolkien" href="/autores/j-r-r-tolkien" />
        <MenuItem texto="George R.R. Margin" href="/autores/george-r-r-martin" />
    </Menu>
    <Menu titulo="Outras Categorias">
        <MenuItem texto="Últimas Notícias" href="/" />
        <MenuItem texto="Séries Populares" href="/" />
        <MenuItem texto="Facebook" href="/" />
        <MenuItem texto="Instagram" href="/" />
        <MenuItem texto="Youtube" href="/" />
    </Menu>
</aside>