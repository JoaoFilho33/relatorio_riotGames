# Engenharia reversa no site da [Riot Games](https://www.riotgames.com/pt-br)
## Relatório da análise do HTML/CSS da página 

### Breakpoints

- Celular: Largura até 959px
- Tablet: Largura de 960 até 1024px
- Desktop: Largura a partir de 1025px

### Grandes Secções

#### sideBar (.riotBar)
Menu Superior - Localizado no topo da página, contém o logotipo da Riot Games, um botão de login e links para as principais páginas do site.
    - Composta por divs principais
        - riotBar-header
            a. Comporta as divs abaixo
        - riotBar-left-content
            a. Logo da Riot Games que fica na extrema esquerda
        - riotBar-center-content
            a. Itens de menu que dão acesso a outras páginas importantes
        - riotBar-hight-conten
            a. Barra de pesquisa + botão "fazer login" que  ficam na extrema direita

#### seção inicial (.hero-new)
    - Composta por duas divs
        - hero-new__background
            a. Uma imagem de background que sofre um corte transversal da esquerda para  direita quando a tela é menor que 960px
        - hero-new__content
            a. Ela possui o nome do boneco que é exibido na imagem, um botão "reserve agora" e a descrição desse boneco. A descrição some quando atinge uma tela menor que 960px 


#### seção novidades (.whats-happening)
    - Composta por duas divs
        - whats-happening__title + botão(ver tudo)
            a. display: flex
            b. justify-content: space-between(colocando "Novidades" e o botão em lados opostos, porém alinhados horizontalmente)
            c. align-itens: center
        - whats-happening__wrapper(conteúdo)
            a. hero-wrapper - Imagem + título da notícia principal
                - Com a tela maior que 1280px a imagem do herói fica ao lado dos articles, menor que isso ela fica acima
            b. _articles
                - Com a tela maior que 1280px as notícias ficam em colunas flex-direction: row. 
                - Com a tela entre 960px e 1280px o card perde a imagem e fica apenas com uma logo. E fazem duas colunas.
                - Menor que 960px a imagem volta a aparecer, E voltam a ficar em apenas uma coluna.

#### Seção Jogos (.our-games)
    - Composta por duas divs
        - _title
            a. text-align: left
        - _wrapper
            a. informa os jogos da riot
            b. display está alinhado com grid centralizando seus itens. Com a tela de celular 960px vira display:flex

    - Ela possui 3 seções "Nossos jogos", "Esportes" e "Entretenimento". E todas seguem o mesmo estilo citado acima.

#### Seção Riot Forge (.product-carousel)
    - Composta por duas divs
        - _title
            a. text-align: left
        - _wraper
            a. É um carrossel com mais informações sobre jogos da riot. Deixa três cards visíveis por vez. Com largura menor que 960px exibe apenas um

#### Seção carreiras (.careers)
    - Composto por duas divs
            a. Descrição, contador "Vagas Abertas", contador "Escritórios", Botão "Explorar carreiras".
            b. Lado a lado com uma imagem. Com um corte transversal como divisória
            c. Tela < 960px o item a(Descrição) fica na parte de cima do item b (imagem)

#### .footer
    - Composto por três divs
        a. Logo da riot na tela > 1280px fica a direira do resto dos links.
        b. Links de acesso a coisas importantes da riot, como parte de suporte, etc
        c. E uma div guardando o link das redes sociais da riot.

    Em telas menores que 960px o rodapé passa a possuir um flex-direction: column.