A forma como a homepage do site se comporta é mais complicada do que a dos outros posts.

Para alterar a homepage do site, siga os passos abaixo:

1 - faça as alterações desejadas no arquivo home.Rmd e salve
2 - depois que o site atualizar, com a função serve site, será gerado um arquivo home.html, que é o output do arquivo home.Rmd que efetivamente seria incluído no site (seria porque esta pasta não altera a home page)
3 - abra o arquivo home.html pelo R
4 - vá em themes\hugo-theme-cleanwhite\layouts\partials e abra o arquivo homepage.html
5 - OBS importante: esse arquivo não existe originalmente no tema cleanwhite do Hugo, ele foi criado por mim (Gabriel) para criar uma homepage personalizada diferente da homepage default do tema, o que significa que se você começar um projeto do zero com esse tema, o arquivo não estará lá
6 - aproximadamente na linha 22 do homepage.html deve haver alguns comentários escrito AQUI VAI O CODIGO HTML DO POST e os códigos html vão até outro blocos de comentário com AQUI ACABA O POST
7 - entre esses dois comentários, apague o que havia antes e cole o código html de home.html, removendo o código --- antes
														 title: Home
														 ---


Assim, você trabalha no arquivo Rmd do jeito usual, o site gera uma versão html do Rmd, colando no arquivo homepage.html você efetivamente atualiza a homepage do site

Obs: Não recomendo tentar usar o output html do próprio Rmd, fica bem ruim