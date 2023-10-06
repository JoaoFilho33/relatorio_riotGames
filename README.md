# Engenharia reversa no site da [Riot Games](https://www.riotgames.com/pt-br)
## Relatório da análise do HTML/CSS da página 

### Breakpoints

- Celular: Largura até 959px
- Tablet: Largura de 960 até 1024px
- Desktop: Largura a partir de 1025px

### Grandes Secções

#### sideBar (.riotBar)
    - Composta por divs principais
        - riotBar-header-wrapper
            a. 
        - riotBar-header
            a. 
        - riotBar-left-content
        - riotBar-center-content
        - riotBar-hight-conten

#### seção inicial (.hero-new)
    - Composta por duas divs
        - hero-new__background
            a.
        - hero-new__content

#### seção novidades (.whats-happening)
    - Composta por duas divs
        - whats-happening__title + botão(ver tudo)
            a. display: flex
            b. justify-content: space-between(colocando "Novidades" e o botão em lados opostos, porém alinhados horizontalmente)
            c. align-itens: center
        - whats-happening__wrapper(conteúdo)
            a. hero-wrapper - Imagem + título da notícia principal
                - display: block
