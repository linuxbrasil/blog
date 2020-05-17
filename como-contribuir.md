---
layout: post
title:  "Como contribuir!"
date:   2020-05-16 21:30:19 -0300
categories: ajuda
author: "Reginaldo"
---
Sejam bem-vindos ao nosso blog!

Estamos muito felizes de compartilhar com vocês os conhecimentos que são discutidos e trocados no nosso grupo.
Nossa [comunidade no Telegram](https://t.me/LinuxParaTodos) tem mais de 3.2k de membros e há troca de mensagens com volumes impressionantes. São abordados temas desde os mais básicos sobre configuração de servidores, LPI, dicas diversas de uso comum em desktop e discussões diversas. Com esse canal vamos publicar materiais que visam a deixar disponível de forma organizada os assuntos abordados.

Se você chegou até aqui está procurando saber como participar do blog e vou tentar ser o mais breve e prático possível.

Estamos usando Jekyll como plataforma para publicação dos artigos, então recomendo dar uma olhada na [documentação](https://jekyllrb.com/) dele para esclarecer dúvidas quanto a como formatar o texto.

Vou mostrar como contribuir em 4 passos sem ter que instalar nada, usando apenas o próprio Github:

**Passo 1.** Acesse com sua conta o [Github](https://github.com) e crie um fork do [projeto](https://github.com/linuxbrasil/blog)

**Passo 2.** Vá até a pasta `_posts` e veja que tem alguns documentos lá com a data e o título como nome. Crie um novo arquivo informando a data e o título (sem acentos e com hífen no lugar dos espaços)

**Passo 3.** No começo do arquivo crie uma tabela e descreva os detalhes do `post` no seguinte formato 

![passo-3](https://snag.gy/fbe8Ag.jpg)

No topo do arquivo você configura conforme a seguir:
 * **layouts**: define o layout desta página, não altere
 * **title**: Título do artigo
 * **header-img**: Aqui vai a sua imagem(que deve ficar no diretório assets/img).
 * **date**: Data da pubicação no formato YYYY-MM-DD HH:MM:SS, o -0200 é o timezone
 * **categories**: Categorias que este artigo pertence, caprixe nisso
 * **author**: Seu nome
 * **author_url**: Um link que você queira postar, para que as pessoas te encontrem, seu portifólio, enfim...
 * **author_ur_label**: O texto ancora para seu link
 * **comments**: habilita e desabilita comentários
 
O Jekyll que faz o build para o HTML fornece alguns recursos legais, como este **code highlight** a seguir:

{% highlight php %}
#!/bin/bash
DIR_ORIG="/diretorio/a/ser/compactado/"
DIR_DEST="/diretorio/a/ser/enviado/o/arquivo"
BKP_NAME="BKP-`date +%Y_%m_%d`.tar.gz"

# compactação do diretório de origem diretamente no diretório de destino
tar -xzvf ${DIR_DEST}${BKP_NAME} ${DIR_ORIG}

# mensagem de resultado
echo "Seu backup foi realizado com sucesso."
echo "Diretório: ${DIR_ORIG}"
echo "Destino: ${DIR_DEST}${BKP_NAME}";
exit 0

{% endhighlight %}


**Passo 4.** Salve o arquivo com o conteúdo e submeta um PR ao repositório principal, indo até a tab de `Pull requests` do seu fork e clicando em `New pull request`

PS.: Não esqueçam de adicionar seu nome e um link no fim do artigo para que quem ler e quiser algum serviço ou trocar uma ideia com vocês, possam encontrá-los.

