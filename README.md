BBBot + OpenCV
===============

Você precisa exportar duas variáveis para poder logar no site da Globo:

```
export GLOBO_USERNAME='your-email@globo.com'
export GLOBO_PASSWORD='xxxxxxxxx'
export PARTICIPANTE=1
```

PARTICIPANTE se refere à posição do participante. Caso ele seja o primeiro da lista, colocar um 1,
o do meio 2 e o último 3.

Requerimentos
==============

Esse bot utiliza o Puppeteer para interagir com a página e o PIL e OpenCV para quebrar os captchas.

- Python3
- Node.JS

Depois de instalar essas duas dependências, rode os seguinte comandos:

```
pip3 install -r requirements.txt
npm install
```

Rodando o bot
==============

```
npm start
```

TODO
=====

  - Precisa melhorar em condições adversas (clique errado, dois cliques no captcha);
  - Colocar no docker.hub;
  - Cleanup das pastas de imagens;
  - Matar o script caso nenhum output seja visto por 10 segundos;

Inspirado no https://github.com/DanielHe4rt/bbbot/ porém usando uma abordagem diferente para quebrar o captcha.
Obrigado! @DanielHe4rt
