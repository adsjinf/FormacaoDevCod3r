<script>
    import Menu from "./Menu.svelte";
    import MenuItem from "./MenuItem.svelte";

    let titulos = ["Navegação", "Principais Autores", "Outras Categorias"];
    let menuItens = [
        ["Início", "Personagem", "Autores", "Séries"],
        ["J.K.Roling", "J.R.R.Tolkien", "George R.R. Martin"],
        [
            "Últimas Notícias",
            "Séries Populares",
            "Facebook",
            "Instagram",
            "Youtube",
        ],
    ];
</script>

<aside
    class="flex flex-col self-start gap-10 w-72 border border-zinc-800 p-5 rounded-md"
>
    <Menu titulo={titulos[0]}>
        <MenuItem texto={menuItens[0][0]} href="/" />
        <MenuItem texto={menuItens[0][1]} href="/" />
        <MenuItem texto={menuItens[0][2]} href="/autores" />
        <MenuItem texto={menuItens[0][3]} href="/" />
    </Menu>
    <Menu titulo={titulos[1]}>
        <MenuItem texto={menuItens[1][0]} href="/autores/j-k-rowling" />
        <MenuItem texto={menuItens[1][1]} href="/autores/j-r-r-tolkien" />
        <MenuItem texto={menuItens[1][2]} href="/autores/george-martin" />
    </Menu>
    <Menu titulo={titulos[2]}>
        <MenuItem texto={menuItens[2][0]} href="/" />
        <MenuItem texto={menuItens[2][1]} href="/" />
        <MenuItem texto={menuItens[2][2]} href="/" />
        <MenuItem texto={menuItens[2][3]} href="/" />
        <MenuItem texto={menuItens[2][4]} href="/" />
    </Menu>
</aside>
