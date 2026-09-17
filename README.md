# Youning
Um app que une o Amplitube 5, o Youtube Music, Youtube e recupera as afinações da musica em um só lugar!

#---- Descrição ----#
O app foi feito com o propósito de facilitar meu aprendizado com a guitarra, onde o caminho para fazer tudo isso acabava sendo muito demorado.

#---- Linguagens ----#
O app resumidamente utiliza SQLite e Python, onde utiliza a API do Songsterr para recuperar as informações das afinações.

#---- Funcionamento ----#
Ao abrir o Youning, ele automaticamente procura o Amplitube 5 instalado nas pastas padrão e adequa o tamanho dele para a janela do app (coisa que o Amplitube 5 não faz de forma nativa).
Caso queira logar com sua conta do google, é totalmente seguro pois ele utiliza um navegador integrado que salva o cache em máquina (o que permite a sessão ficar ativa sempre e utilizar o Yt Premium).
Ao escolher uma música, ele faz duas verificações do nome, acessa a API para recuperar a afinação (por exemplo D A D G B E), faz uma leitura do SQLite e verifica se a música está salva, caso esteja ele apenas recupera as informações da música sendo: Artista, Musica, Afinação, Cordas, Fonte.
Caso não esteja, ele salva a música no banco de dados para uma recuperação futura mais rápida (caso queira tocar a mesma música novamente).

#---- Interface ----#
O Youning tem uma interface simples, apenas sendo exposto o necessário e fazendo parte do tema do Youtube Music (ficando de forma homogênea e agradável). Informa o nome da música, a afinação, as cordas necessárias e a fonte sendo padrão Songsterr.

#---- Imagens ----#
Em algumas imagens repare em detalhes, como o ícone da conta Google (sem perder o login por cerca de 7 dias, pois a guitarra está no luthier e não abri o Youning). Outras observações são referentes a janela que pode ser expandida da forma que desejar.

Verifique também o arquivo SQLite que consta a música teste que estava ao finalizar o Youning e testar pela primeira vez.


#---- Informações adicionais ----#
Iria utilizar o MySQL porém seria necessário um servidor ou abrir uma porta para meu computador. Realizei alguns testes e o funcionamento era o mesmo (apenas pela parte que tenho mais afinidade com o SQL Workbench), optei por trocar para SQLite pois também tenho amigos que tocam e o Youning com certeza ajuda a agilizar um pouco, já que o Amplitube já conta com o afinador embutido.
O projeto em si foi feito com intuito pessoal, porém nesse momento estou estudando tunelamento de dados, protocolos de rede e formas de blindar o servidor cada vez mais.
