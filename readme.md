## INTRODUÇÃO

Este documento apresenta a documentação do projeto Lança Perfume, um site front-
end de uma loja de moda feminina, desenvolvido com HTML5 e CSS3 como atividade
prática da unidade curricular de Projeto Front-end. A documentação foi elaborada no âmbito
da unidade curricular de Versionamento e colaboração, sob responsabilidade do professor
Josué Rodrigo Evangelista Figueirêdo.
O texto está organizado em seis partes: identificação do projeto, apresentação,
funcionalidades, tecnologias utilizadas, estrutura de arquivos e instruções de execução,
seguidas da demonstração das páginas e das propostas de melhorias futuras.

## IDENTIFICAÇÃO DO PROJETO
O Quadro 1 reúne as informações de identificação do projeto, da equipe e da unidade
curricular.
Quadro 1 – Identificação do projeto
Item Informação
Nome do projeto Lança Perfume
Integrantes da equipe [Nome 1], [Nome 2], [Nome 3] (preencher)
Curso e turma [Nome do curso] – Turma IFTP
Professor responsável Josué Rodrigo Evangelista Figueirêdo
Unidade curricular da
documentação

Versionamento e colaboração

Material de design Projeto de design elaborado na plataforma Canva [inserir link]
Fonte: Elaborado pelos autores (2026).
3 APRESENTAÇÃO DO PROJETO
3.1 O que é o projeto

O Lança Perfume é um site de vitrine virtual (catálogo online) de uma loja de moda
feminina. Ele reúne a página inicial da coleção Primavera 27, quatro páginas de catálogo por
categoria de produto (bolsas e calçados, vestidos e macacões, blusas e t-shirts, casacos e
blazers) e uma página de outlet.

3

3.2 Objetivo principal
O objetivo é apresentar os produtos e as campanhas da marca de forma visual e
organizada, permitindo que o visitante navegue facilmente entre as categorias, tanto no
computador quanto no celular.
3.3 Problema que busca resolver

Uma loja de moda precisa mostrar seus produtos de maneira atrativa e fácil de
explorar. O projeto resolve essa necessidade ao oferecer um site com navegação simples,
layout limpo em preto e branco (que valoriza as fotos dos produtos) e organização dos itens
por categoria, evitando que o cliente precise procurar peça por peça.

3.4 Justificativa

O projeto foi desenvolvido como atividade prática da unidade curricular de Projeto
Front-end, com a finalidade de aplicar conhecimentos de HTML e CSS, tais como
estruturação de páginas, layout com Flexbox, posicionamento de elementos, navegação entre
páginas e adaptação do layout para telas de celular.
4 FUNCIONALIDADES

4.1 Funcionalidades implementadas

Foram implementadas as seguintes funcionalidades:
a) página inicial (lp.html), com banner principal da campanha, faixa com destaques
de produtos, imagem da coleção Primavera 27 e menu de navegação por
categorias;
b) faixa de cupom no topo de todas as páginas, exibindo a mensagem de primeira
compra com o cupom WELCOMELP (15% OFF), de caráter apenas informativo,
pois não existe carrinho ou etapa de pagamento para aplicá-lo;
c) menu de navegação no cabeçalho (Primavera, Categorias, Bolsas e Calçados,
Outlet), presente em todas as páginas;

4

d) barra “Navegue por categoria” no final de cada página, com links para Início,
Bolsas e Calçados, Vestidos e Macacões, Blusas e T-shirts, Casacos e Blazers e
Outlet;
e) quatro páginas de catálogo, com grade de fotos dos produtos organizadas por
categoria;
f) página Outlet, com o destaque “LP – 20 anos”, QR Code para download do
aplicativo e ícones das redes sociais (Instagram, Pinterest, TikTok e WhatsApp)
no rodapé;
g) layout responsivo para celular: abaixo de 485 px de largura, o layout se
reorganiza, com menu superior oculto, imagem principal própria para dispositivos
móveis e elementos dispostos em coluna;
h) rolagem suave ao clicar em links internos e transição suave entre páginas (@view-
transition), em navegadores que suportam esse recurso.

4.2 Ações disponíveis ao usuário
No sistema, o usuário consegue:
a) navegar entre as seis páginas do site pelo menu do cabeçalho ou pela barra de
categorias;
b) visualizar as fotos dos produtos de cada categoria;
c) conhecer a campanha da coleção Primavera 27 e a promoção de primeira compra;
d) acessar o site pelo celular com o layout adaptado.

4.3 Funcionalidades não implementadas
O site é estático. Não há carrinho de compras funcional (o ícone da sacola é apenas
uma imagem), login, busca, filtros, página de detalhes de produto nem pagamento. Os ícones
das redes sociais também não possuem links ativos.
5 TECNOLOGIAS UTILIZADAS

O Quadro 2 apresenta as tecnologias empregadas e o respectivo uso no projeto.
Quadro 2 – Tecnologias utilizadas no projeto
Tecnologia Uso no projeto

5

HTML5 Estrutura de todas as páginas
CSS3 Estilização, escrita dentro da tag &lt;style&gt; de cada página
Flexbox Organização do layout (cabeçalho, grades de produtos e menus)
Media Queries Adaptação do layout para celular (max-width: 485px)
Git Controle de versão do código
GitHub Hospedagem do repositório e trabalho em equipe
Canva Material de design do projeto
Fonte: Elaborado pelos autores (2026).
O projeto não utiliza JavaScript, frameworks nem bibliotecas externas.

## ESTRUTURA DO PROJETO

A Figura 1 mostra a organização de pastas e arquivos do projeto.
Figura 1 – Estrutura de pastas e arquivos do projeto
lança-perfume/
├── lp.html # Página inicial (Primavera 27)
├── bolsas-e-calçados.html # Bolsas, calçados e acessórios
├── vestidos-e-macacões.html # Vestidos e macacões
├── blusas-e-tshirts.html # Camisas, blusas e t-shirts
├── casacos-e-blazers.html # Casacos, jaquetas e blazers
├── outlet.html # Página Outlet &quot;LP - 20 anos&quot;
├── README.md # Documentação do projeto
├── screenshots/ # Capturas de tela do README
└── assets/ # Imagens do site
├── main.jpg, main-mobile.jpg, main2.jpg, sub-main2.jpg
├── *-faixa.png # Faixa de destaques
├── sacola.png # Ícone da sacola
├── bolças e calçados/
├── vestidos e macacões/
├── camisetas e t-shirts/
├── camisas e blazers/
└── outlet/ # Modelos, QR Code e redes sociais
Fonte: Elaborado pelos autores (2026).
Os principais arquivos e diretórios são descritos a seguir:
a) lp.html: porta de entrada do site, com banner, destaques e acesso às categorias;
b) páginas de catálogo (bolsas-e-calçados, vestidos-e-macacões, blusas-e-tshirts e
casacos-e-blazers): exibem as fotos dos produtos de cada categoria em linhas de
imagens;
c) outlet.html: página promocional com QR Code do aplicativo e redes sociais;
d) assets/: todas as imagens usadas pelas páginas, separadas por categoria.

6

## COMO EXECUTAR O PROJETO
O projeto é feito apenas com HTML e CSS, portanto não requer instalação de
programas nem configuração de servidor. O único pré-requisito é um navegador atualizado,
como Google Chrome, Microsoft Edge, Firefox ou Safari.
Para executar o projeto, devem ser seguidos os passos abaixo:
1. baixar o projeto pelo GitHub, clicando em Code e depois em Download ZIP,
extraindo a pasta em seguida; ou clonar o repositório pelo terminal, com o
comando a seguir;
git clone &lt;link-do-repositório&gt;
2. abrir a pasta do projeto;
3. dar dois cliques no arquivo lp.html (ou clicar com o botão direito, escolher Abrir
com e selecionar o navegador);
4. navegar pelo site usando o menu. Para ver a versão mobile, reduzir a largura da
janela para menos de 485 px ou usar o modo de dispositivo das ferramentas do
desenvolvedor (tecla F12).
Importante: a pasta assets deve ser mantida no mesmo local dos arquivos .html; caso
contrário, as imagens não serão exibidas.

## DEMONSTRAÇÃO DO PROJETO

As capturas de tela das páginas estão disponíveis na pasta screenshots do repositório.
O Quadro 3 resume o que cada uma delas apresenta.
Quadro 3 – Páginas demonstradas no projeto
Página Descrição
Página inicial (computador) Banner da campanha, faixa de destaques e imagem da coleção Primavera

27

Página inicial (celular) Versão adaptada para telas pequenas, com imagem principal própria para

mobile

Bolsas e Calçados Catálogo com sandálias, botas, bolsas, carteiras, bonés e cintos
Vestidos e Macacões Catálogo de vestidos curtos, midi e longos e macacões
Blusas e T-shirts Catálogo de camisas, camisetas e t-shirts de diferentes modelagens
Casacos e Blazers Catálogo de jaquetas, parkas, casacos e blazers
Outlet Página “LP – 20 anos” com QR Code para o aplicativo e ícones das redes

sociais

7

## *MELHORIAS FUTURAS*
Como evolução do projeto, propõem-se as seguintes melhorias:
a) separar o CSS em um arquivo próprio (por exemplo, css/style.css), pois hoje cada
página tem seu CSS dentro do HTML e partes do código (cabeçalho, menu, barra
de categorias) se repetem, o que um arquivo único facilitaria na manutenção;
b) adicionar JavaScript para um carrinho funcional, permitindo adicionar produtos,
ver o total e aplicar o cupom WELCOMELP, hoje apenas informativo;
c) criar páginas de detalhe de produto, com nome, preço, tamanhos disponíveis e
várias fotos, e adicionar filtros por categoria, cor e preço;
d) melhorar a acessibilidade, incluindo o atributo alt nas imagens, usando tags
semânticas e garantindo bom contraste e navegação por teclado;
e) ampliar a responsividade, já que hoje há ajuste apenas para telas de até 485 px,
incluindo pontos de quebra para tablets e telas grandes;
f) corrigir pequenos erros de texto e organização, como “cumpo” (cupom),
“dowload” (download) e “OFICIAS” (oficiais), além de ativar os links das redes
sociais na página Outlet.

## *CONSIDERAÇÕES FINAIS*
O Lança Perfume cumpre o objetivo de apresentar uma vitrine virtual organizada por
categorias, com navegação simples e layout adaptado ao celular, aplicando na prática os
conceitos de HTML, CSS, Flexbox e Media Queries. As limitações identificadas, como a
ausência de carrinho, busca e filtros, indicam caminhos claros para a evolução do projeto, e o
uso de Git e GitHub apoia o trabalho colaborativo e o versionamento das próximas etapas.