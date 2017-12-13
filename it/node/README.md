![picture alt](../img/logos/node.png "Title is optional")
# Node
- - - -
## O que é Node.js?
[https://nodejs.org](https://nodejs.org)
**Node.js** Como um tempo de execução do JavaScript conduzido por eventos assíncronos, o Node foi projetado para criar aplicativos de rede escaláveis. No seguinte exemplo "hello world", muitas conexões podem ser tratadas simultaneamente. Em cada conexão, o retorno de chamada é disparado, mas se não houver nenhum trabalho a ser feito, o Node dormirá.

```js
    const http = require('http');

    const hostname = '127.0.0.1';
    const port = 3000;

    const server = http.createServer((req, res) => {
    res.statusCode = 200;
    res.setHeader('Content-Type', 'text/plain');
    res.end('Hello World\n');
    });

    server.listen(port, hostname, () => {
    console.log(`Server running at http://${hostname}:${port}/`);
    });
```

Se você trabalhou com o JavaScript por um tempo, talvez tenha ouvido falar de **npm**.
**npm** facilita que os desenvolvedores JavaScript compartilhem o código que criaram para resolver problemas específicos e para outros desenvolvedores reutilizar esse código em seus próprios aplicativos.

Uma vez que você esteja dependendo deste código de outros desenvolvedores, **npm** facilita verificar se eles fizeram alguma atualização e baixar essas atualizações quando elas são feitas.

Esses bits de código reutilizável são chamados de pacotes ou módulos. Um pacote é apenas um diretório com um ou mais arquivos nele, juntamente com um arquivo chamado "package.json" que contém metadados sobre o pacote. Um aplicativo típico, como um site, dependerá de dezenas ou centenas de pacotes. Esses pacotes são geralmente pequenos; a idéia geral é que você crie um pequeno bloco de construção que resolva bem um problema. Isso permite que você compile soluções personalizadas maiores desses pequenos blocos de construção.

>**Há muitos benefícios para isso; Isso permite que sua equipe se baseie na experiência fora de sua organização trazendo pacotes de pessoas que se concentraram em áreas problemáticas específicas. Mesmo que você não reutilize o código de pessoas fora de sua organização, usar esse tipo de abordagem baseada em módulo pode ajudar sua equipe a trabalhar melhor e tornar possível reutilizar o código em todos os projetos.**

Você pode encontrar pacotes para ajudá-lo a criar seu aplicativo navegando no site **npm**. Quando você está navegando no site, você encontrará muitos módulos de nó.
**npm** começou como o gerenciador de pacotes do Nó, então você encontrará muitos módulos que podem ser usados ​​no lado do servidor. Há também muitos pacotes que adicionam comandos para você usar na linha de comando.
Você também encontrará pacotes que podem ser usados ​​no front-end.
- - - -
### Como é composta
**npm** é composta por três peças distintas:
    **1.** O site
    **2.** O registro 
    **3.** E a CLI

**1.** _O site_
    serve como a ferramenta principal para que os usuários descubram pacotes
**2.** _O registro_
    é um grande banco de dados de informações sobre pacotes
**3.** _E a CLI_ 
    é como os desenvolvedores publicam seus pacotes no registro ou baixam pacotes que desejam instalar.

#### CONCLUSÃO

**npm** é uma maneira de reutilizar o código de outros desenvolvedores, e também uma maneira de compartilhar seu código com eles, e facilita a gestão das diferentes versões do código.

- [npm](#npm)
    - [O que é npm?](#o-que-%C3%A9-npm)
        - [Como é composta](#como-%C3%A9-composta)
            - [CONCLUSÃO](#conclus%C3%A3o)