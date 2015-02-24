---
layout: post
title: Windows, porque não usar
snip:  Para desenvolvedores
---

![Vim](http://cdn.instantshift.com/media/uploads/2013/04/universal-mobile-site-design-flaw.jpg)

***A recomendação é simples:*** 

Não use Microsoft Windows se não for necessário como máquina de desenvolvimento de qualquer coisa que não seja Java,.Net ou C#. É óbvio que .NET funciona porque foi feito para Windows. No caso do Java, tudo é feito para rodar dentro da JVM. Até mesmo porque os scripts de linha de comando são sempre chamados pelo ```java -jar xxx.jar```.

> Segundo o Ph.D em Ciência da Computação e mestre em Engenharia de Software, Diomidis Spenillis autor de livros como ***[Code Reading](http://www.amazon.com/Code-Reading-Open-Source-Perspective/dp/0201799405)*** livro este que é dirigido a programadores que desejam melhorar seus códigos e técnicas para códigos escritos de outras pessoas, Spenillis explica que a arquitetura do Windows Application Programming Interface (API) é demasiadamente difícil de dominar e utilizar de forma eficaz, e contribui negativamente para a segurança, robustez e portabilidade das aplicações desenvolvidas sob ele.

Você poderá encontrar esta citação de Spenillis, no paper ***[Standards & Computer Interfaces](http://www.sciencedirect.com/science/article/pii/S0920548998000129)***.

Perl, PHP,Ruby, Python e outros interpretadores nasceram no ambiente Unix e dependem de APIs ***[POSIX](http://en.wikipedia.org/wiki/POSIX)*** por baixo. Distribuições GNU/Linux, BSD/Darwin (OS X) implementam essa família de padrões e seguem a filosofia UNIX. O Windows, obviamente, não é UNIX e muito menos POSIX. Existe, porém, como ter o sub-sistema POSIX sobre o Windows como o projeto ***[Cygwin](https://www.cygwin.com/)*** e o projeto ***[Windows Services for UNIX](http://www.microsoft.com/en-us/download/details.aspx?id=274)***. Apesar do grande esforço desses projetos em tentar prover as mesmas APIs POSIX, existem hoje diferenças nos ambientes GNU/Linux e Darwin que eles não cobrem, e por isso muita coisa ainda vai quebrar. É um trabalho absurdo tentar fazer o Windows ficar compatível com um ambiente UNIX inteiro. 

> A aplicação melhor sobrevive a plataforma na qual foi desenvolvido e implantado - ***[OPENNT: UNIX Application Portability to Windows NT via an Alternative Environment Subsystem](https://www.usenix.org/legacy/publications/library/proceedings/usenix-nt97/full_papers/walli/walli.pdf)- Stephen R.Walli***

Ainda segundo Stephen R.Walli, a melhor alternativa neste caso, seria usar o Windows NT. O problema é que o Windows NT que tem suporte ao sub-sistema POSIX, é a versão anterior ao NT 5.1. Ou seja, uma versão anterior ao Windows XP e Windows Server 2003. A partir da versão 5.1 em diante, a Microsoft resolveu substituir o sub-sistema POSIX pelo então já citado ***[Windows Services for UNIX](http://www.microsoft.com/en-us/download/details.aspx?id=274)***. Esta informação você poderá conferir no ***[http://support.microsoft.com/kb/308259](http://support.microsoft.com/kb/308259)***. Basicamente, tudo relacionado a POSIX e Microsoft, você encontrará no NT anterior a versão 5.1 como destaca David G.Korn no paper ***[UWIN-Unix for Windows](https://www.usenix.org/legacy/publications/library/proceedings/usenix-nt97/full_papers/korn/korn.pdf)***.

> "Mas eu desenvolvo em PHP e Python no Windows sem problemas!"

O problema é que sempre irá depender de gambiarras para fazer uma ferramenta que é simples no UNIX, funcionar bem no Windows. O mesmo para Ruby que funcionará parcialmente bem, o mesmo para Python, Perl, Php e sempre se manterá assim, tudo funcionando em parte, nunca 100%. Sem falar do conjunto de ferramentas disponíveis em sub-sistemas POSIX. Veja o exemplo a baixo de algumas destas ferramentas:

* ***Arquivo e gestão de projetos*** - ls , find , grep/ack , bash
* ***Ferramentas de edição de texto*** - vim , awk , type , column
* ***Compiler e / ou interpretador*** - gcc , perl, python
* ***Construir grupos de programas*** - make
* ***Debugger*** - gdb , valgrind , ltrace , lsof , pmap
* ***Controle de versão*** - diff , patch , svn , git

Não vou dizer que sistemas baseados em Unix são sempre a melhor alternativa para qualquer tarefa de programação; é, sem dúvida, muito mais adequado para C, C++, Python, Perl, Ruby, PHP, ou desenvolvimento Shell do que para linguagens como Java, .NET ou C#, especialmente quem escreve aplicações baseadas em GUI. Particularmente, não estou tentando convencê-lo a parar de usar o seu Visual Studio. Cada um faz o que desejar e como desejar.

Mas, afinal, empresa séria apoiaria este tipo de postura? Bem, o Google está substituindo todos os seus ambientes de trabalho por GNU/Linux e BSD/Darwin (OS X) por questões de segurança como também praticidade. Na verdade, o Google nunca foi realmente dependente da plataforma Microsoft Windows, por isso, esta é uma "solução" de fácil implementação dado ao fato de que o desenvolvimento de boa parte dos softwares por lá é Open-Source, e toda sua linha de aplicações de negócios são baseados em Cloud.  

> Mas em meu trabalho, sou obrigado a usar Microsoft Windows. Logo tenho que ser neutro, não há alternativas por lá.

Nesse caso, existe sim uma alternativa. Como por exemplo, o uso de máquinas virtuais com a ajuda do bom e velho ***[Vagrant](https://www.vagrantup.com/)***. Se você é o tipo de profissional ou estudante com "mente aberta", está mais do que na hora de experimentar algo novo. No fim das contas, você estará usando um sistema que lhe ajudará a dar passos significativos para melhorar à sua maneira de desenvolver software, estará evitando a pirataria, e descobrindo um novo universo de possibilidades.

Recomendação:
<dl>
	<dt><a href="http://blog.sanctum.geek.nz/unix-as-ide-editing/">Unix as IDE editing</a></dt>
</dl>
