<h1>Projeto de Página Web Responsiva
</h1>

<p>Este projeto é uma página web responsiva criada com HTML, CSS e JavaScript. A página possui um menu de navegação interativo e adaptável a diferentes tamanhos de tela. Além disso, a página inclui seções como "Sobre Nós", "Cardápio" e "Contatos", com estilo e animações aplicadas para melhorar a experiência do usuário.

</p>

<h2>Funcionalidades</h2>
<p>• <b>Menu de navegação:</b> O menu de navegação é fixo e inclui links de navegação, com destaque visual ao passar o mouse.</p>
<p>• <b>Responsividade:</b> O layout da página é adaptável a diferentes dispositivos, com ajustes para telas pequenas e médias.</p>
<p>• <b>Efeitos interativos:</b> O menu pode ser expandido e contraído ao clicar no ícone de menu, proporcionando uma navegação dinâmica.</p>


<h2>Tecnologias Utilizadas</h2>
<p>• <b>HTML5</b> - Estrutura da página</p>
<p>• <b>CSS3</b> - Estilos e responsividade</p>
<p>• <b>JavaScript</b> - Funcionalidade de interatividade para o menu
</p>


<h2>Exemplo de Uso
</h2>
<h3>Estrutura HTML</h3>

```
<div class="content">
    <div class="logo">
        <img src="logo.png" alt="Logo">
        <h3>Logo</h3>
    </div>
    <div class="menu-toggle">
        <span></span>
        <span></span>
        <span></span>
    </div>
    <ul class="list-menu">
        <li><a href="#">Home</a></li>
        <li><a href="#">Sobre</a></li>
        <li><a href="#">Cardápio</a></li>
        <li><a href="#">Contato</a></li>
    </ul>
</div>

```

<h3>CSS para Menu Responsivo</h3>

```
.menu-toggle {
    display: none;
}

@media (max-width: 720px) {
    .menu-toggle {
        display: block;
        cursor: pointer;
    }

    .list-menu {
        display: none;
    }

    .content.on .list-menu {
        display: flex;
        flex-direction: column;
    }
}

```

<h3>JavaScript para Menu Toggle</h3>

```
let show = true;
const menuContent = document.querySelector('.content');
const menuToggle = menuContent.querySelector('.menu-toggle');

menuToggle.addEventListener('click', () => {
    menuContent.classList.toggle('on', show);
    show = !show;
});

```


<h2>Personalizações</h2>
<p>Você pode personalizar este projeto de acordo com suas necessidades:</p>


<p>• <b>Alterar o conteúdo:</b> Modifique os links do menu e os textos nas seções conforme necessário.</p>
<p>• <b>Personalizar o estilo:</b> O CSS pode ser facilmente ajustado para refletir sua identidade visual.</p>














