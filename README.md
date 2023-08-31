
Documentação do Projeto Pokedex
HTML (index.html)
Descrição:
Este arquivo HTML é a página principal da Pokedex, onde os detalhes dos pokémons são exibidos. Ele contém a estrutura da página, estilos importados e links para os scripts JavaScript que controlam a funcionalidade da aplicação.

Elementos Principais:
<link>: Importa folhas de estilo externas para a página.
<section class="content">: Contém o conteúdo principal da Pokedex.
<h1>: Título principal da Pokedex.
<ol id="pokemonList">: Lista ordenada onde os detalhes dos pokémons serão exibidos.
<button id="loadMoreButton">: Botão "Load More" para carregar mais pokémons.
<script>: Inclui os scripts JavaScript necessários para a funcionalidade da página.
JavaScript (pokemon-model.js)
Descrição:
Este arquivo define a classe Pokemon, que representa um objeto Pokémon com várias propriedades para armazenar informações sobre o número, nome, tipos e foto do Pokémon.

Classe:
Pokemon: Classe para criar objetos que representam pokémons com detalhes básicos e informações da API.
JavaScript (poke-api.js)
Descrição:
Este arquivo fornece funções para interagir com a API de Pokémon, obtendo informações detalhadas sobre os pokémons e convertendo essas informações em objetos Pokémon utilizáveis.

Funções Principais:
convertPokeApiDetailToPokemon(pokeDetail): Converte os detalhes da API de um pokémon em um objeto da classe Pokemon.
pokeApi.getPokemonDetail(pokemon): Obtém os detalhes completos de um pokémon específico da API.
pokeApi.getPokemons(offset, limit): Obtém uma lista de pokémons da API com informações básicas e detalhes completos.
JavaScript (script.js)
Descrição:
Este arquivo controla a interação com a API de Pokémon e a renderização dos pokémons na página HTML. Ele também gerencia a ação do botão "Load More" para carregar mais pokémons.

Funções Principais:
loadPokemonItens(offset, limit): Carrega pokémons da API e os renderiza na página.
EventListener do botão "Load More": Responde ao clique do botão para carregar mais pokémons.
