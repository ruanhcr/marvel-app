# Marvel App
App que exibe personagens da Marvel através da [Marvel API](https://developer.marvel.com).
<br>Para o funcionamento da API primeiramente é necessário se inscrever no portal para obter acesso as chaves individuais: "Your public key" e "Your private key".
<br>O app utiliza a biblioteca [Retrofit](https://square.github.io/retrofit/) para fazer requisições para a API, onde são feitas requisições [GET CHARACTERS](https://gateway.marvel.com/v1/public/characters/) para exibir os personagens e [GET COMICS](https://gateway.marvel.com/v1/public/characters/{characterId}/comics/) 
para exibir os comics em que o personagem está contido.
<br>É utilizado no projeto a arquitetura MVVM, juntamente com o [State Flow](https://developer.android.com/kotlin/flow/stateflow-and-sharedflow#stateflow), Injeção de dependência com o [Hilt](https://developer.android.com/training/dependency-injection/hilt-android?hl=pt-br), [Coroutines](https://developer.android.com/topic/libraries/architecture/coroutines?hl=pt-br) do Kotlin, 
[Navigation Component](https://developer.android.com/guide/navigation/navigation-getting-started), além do [Room](https://developer.android.com/jetpack/androidx/releases/room?hl=pt-br) para acessar o banco de dados para marcar e/ou excluir personagens dos favoritos.
<br>As Views são dividas em Home, Pesquisar e Favoritos através de Fragments usando Navigation Bottom, aplicadas em RecyclerView.
<br>A exibição das imagens é feita através da biblioteca [Glide](https://github.com/bumptech/glide).
<br>É possivel ainda fazer a busca pelo personagem na aba de Pesquisa.

<br>![exemplo](https://media3.giphy.com/media/Js3taw30ZXrufAOhbx/giphy.gif?cid=790b761170bcfae8c899d548620f1e09f111875b1a48ba13&rid=giphy.gif&ct=g)
