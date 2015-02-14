---
layout: post
title: Vim é o poder
snip:  IDE pra quê? 
---

![Vim](https://lh4.googleusercontent.com/-8KE515yD9dc/UHfXZ13tSsI/AAAAAAAAA_E/Ao3eToSQPLE/w800-h800/full-screenshot.png)

O Vim é um editor de texto extremamente configurável, criado para permitir a edição de textos de forma eficiente. Também é um melhoramento do editor vi, um tradicional programa dos sistemas UNIX. Possui uma série de mudanças em relação a este último. O próprio slogan do vim é "Vi IMproved". Ou seja, Vi Melhorado. O Vim é tão conhecido e respeitado entre programadores, e tão útil para programação, que muitos o consideram uma verdadeira IDE. 

A primeira semana com o Vim, geralmente, é dolorosa para todo mundo. Portanto, não desanime. Se adaptar ao modal-editing (isto é, ter que ativar um modo especial sempre que você quer inserir texto no arquivo) pode parecer uma tarefa desnecessária e até impossível para o que você precisa para programar. A ideia de trabalhar a esta maneira só ficará mais clara para você depois de alguns dias lutando contra o teclado. Aliás, a grande maioria das coisas do Vim aparentemente não fazem sentido algum no início, mas com o uso fica claro como cada detalhe contribuí para torná-lo um editor de texto incrivelmente ágil e prático.

Muita gente não entende a necessidade de migrar de um editor de texto “normal” para o Vim. Para isso, entender a filosofia dele é fundamental. A ideia básica do Vim é permanecer sempre com as mãos na parte central do teclado. Assim gasta-se menos tempo com deslocamentos desnecessários das mãos e sim com a edição em si. Embora pareça complicado no início não usar o mouse e nem as setas, é isso que torna o Vim tão eficaz.

> Vim te faz sentir como um cirurgião de texto; Você opera precisamente e de forma inequívoca. É uma espécie muito direcionada de comando conjunto. - *Tom Ryder*


# Editores modernos 
Vivemos em um tempo em que há uma grande variedade de editores que são usados para inúmeros fins. Como é o caso do Atom **[https://atom.io](https://atom.io)**. Este é um editor que foi fortemente baseado no **[SublimeText](www.sublimetext.com)** sendo o Sublime hoje considerado por muitos, como o melhor editor para desenvolvedores. Ao observar este quadro, surge uma preocupação: **longevidade**. Parece que passamos uma grande quantidade de tempo nos comprometendo com teclas atalhos, manuais, tutoriais para aprender a manuzear recursos que são específicos para o que estamos usando em um determinado editor e ao mesmo tempo, nos perdendo com a variedade absurda de ferramentas oferecidas nos mais variados editores.

Tanto o Atom, quanto o SublimeText, por exemplo, misturam uma interface gráfica ao lado de uma necessidade de codificação simples. Esta necessidade, na verdade, surgiu como alternativa a editores pesados como é o caso do Adobe DreamWeaver ( largamente usado na década de 90 e por algumas pessoas ainda hoje ). Ou algo como o Eclipse que pode incluir tudo o que você possa imaginar...talvez até algo como... ```uma pia de cozinha!?```

O fato é que nem Sublime, nem Atom, são tão leves e *onipresentes* quanto o VIM. Basicamente, o VIM está disponível por padrão até em sistemas operacionais mais antigos e roda em todos os sistemas que podem implementar a biblioteca C padrão ```você conhece algum S.O que não pode?``` "ou o VI que muda somente alguns comandos" mas que carrega a mesma essência.

IDEs e editores de textos estão entre os grandes motivadores de Guerras Santas entre desenvolvedores. Não vou falar que você deve usar um ou o outro. Produtividade é muito subjetivo e pessoal, não existem regras que torna algo produtivo ou não, tem quem goste de trabalhar ouvindo música, tem quem goste de usar bermuda, e por ai vai.

Já imaginou trabalhar em um editor que pode ser moldado a todas as suas necessidades como desenvolvedor? bem, o VIM oferece esta proposta. Por padrão, o VIM vem igual para todos os usuários. Exceto quando você resolve modificar o seu próprio ```.vimrc``` file. Isto é, existe um arquivo com suas próprias configurações ( seja alguma mudança de hotkey "tecla atalho", configuração de comportamento específico, plugins, funções, modelos e padrões estabelecidos por você ).

# Plugins 

Levando em conta que o Vim existe a mais de 20 anos e que antes mesmo de sua primeira versão em 1988 já existia o VI, fica realmente difícil de especular quantos plugins, addons, scripts devem existir para este editor. O que posso garantir, é que há uma imensa probabilidade de que tudo o que você necessita em um ambiente como no caso de uma IDE, já exista para Vim. A baixo selecionei os plugins mais **"mother fuckers"** que conheço e que merecem um certo destaque neste artigo:

---

### Fugitive

O Fugitive é nada mais, nada menos, do que o mais completo plugin para gerenciamento de projetos git que ja tive o prazer de conhecer. Seu nome se deve à descrição que seu criador **[Tim Pope](http://tpo.pe/)** teve no processo de desenvolvimento da ferramenta: 

> "Fugitive é um plugin git tão impressionante, que deveria ser ilegal".

Éntão foi assim que Pope descreveu seu plugin.

Desde que comecei a usar git há alguns anos atrás, fui muito feliz em preferir usar linha de comando. Afinal, pode assustar a algumas pessoas mas, definitivamente trabalhar com o terminal aumenta significamente a minha produtividade. E interagir com meu git repository dentro do editor em questão, foi uma outra necessidade que surgiu com o tempo.

Em termos práticos, suponhamos que eu deseje descobrir quem foi o responsável por "cagar" o sistema modificando uma determinada linha de código do projeto que está sendo construído no ambiente de desenvolvimento que trabalho. Obter estas informações por linha de comando no terminal, é possível mas requer um pouco mais de trabalho. Basicamente, tenho que lembrar o nome e o caminho do arquivo que estou trabalhando para que possa passa-lo como um argumento para o comando ```git blame```.

Ai que entra o fugitive com o comando ```:Gblame``` que faz exatamente o que eu quero. Isto é, não tenho que recordar o caminho do arquivo atual porque o editor sabe exatamente o caminho. Não tenho que navegar até a linha atual, pois, já estarei lá. Apenas tenho que executar o comando ```:Gblame``` e pimba! feito! Receberei o nome do autor da cagada junto à linha de código. 

No entanto, raramente uso o ```:Gblame```, e a linha de comando sempre foi bom o suficiente para a maioria das tarefas que executo diariamente com o git. Então, por muito tempo, tive o fugitive instalado mas não o usava. Sempre tive uma sensação incômoda de que estava perdendo muito com isto. Afinal, Tim Pope costuma dizer:

> "Eu não vou mentir para você, fugitive.vim pode muito bem ser o melhor wrapper git de todos os tempos." 

Então decidi que valeria a pena cavar mais fundo e compartilhar o que aprendi até aqui embora não seja capaz de cobrir todos os recursos do Fugitive. Sendo assim, vou focar nos que mais uso e achei mais interessantes. Então vamos lá:

- **Complemento a linha de comando git**
Comandos como ```:Gremove``` e ```:Gmove``` mapeia diretamente para git rm e mv git. Eu não me interessava muito por estes comandos porque não me imporatava com os comandos do git. Mas com o tempo as coisas podem ficar realmente confusas se você executar esses comandos no shell quando os ficheiros já estão abertos em seu editor. Por exemplo, se você executar:

{% highlight bash %}
git mv origem/path.txt destino/path.txt 
{% endhighlight %} 

Quando você alternar para o editor e tentar editar o arquivo origem/path.txt note que ele não existirá mais. Usando o ```:Gmove```, no entanto, o comando manterá as coisas arrumadas lidando simultaneamente com o git index e buffers do vim. 

- **Trabalhando com o git index**
Sempre tive uma ideia um pouco difusa do que é o git index. Talvez seja porque o arquivo .git/index usa um formato binário, tornando-se aparentemente inacessível para um editor de texto qualquer. Mas confesso que esta é uma situação interessante onde o Fugitive age brilhantemente. Por exemplo, você poderá usar o comando ```:Gdiff``` para comparar a cópia anterior do seu trabalho com a atual. O modo diff do Vim torna possível encenar interativamente pedaços de cada mudança, como quando você executa o ```git diff --patch``` na linha de comando do terminal. Outra vantagem de usar o ```:Gdiff```, é para resolver os conflitos de mesclagem que costumo lidar com o ```git merge``` .

- **Navegando no git objects database**
Confesso que sempre gostei bastante da interface web que o github fornece. Pois, nela é possível navegar em cada repositório git e ao mesmo tempo lhe fornecem uma URL para cada git object incluindo trees, blobs, tags e commits. O Fugitive neste caso torna possível ler qualquer git object em um buffer, executando o comando ```:Gedit SHA```. Mas não para por aí. EM um buffer commitado, você pode pressionar **Enter** com o cursor em qualquer outro SHA e ele abrirá automaticamente o objeto em um buffer. Estes buffers são tão interativos como uma página da web, e estando no Vim, isto se torna tão prático que nós nunca precisaremos sequer usar o mouse.

Se ainda sim você preferir compartilhar um link para o objeto que você tenha aberto no Vim, o comando ```:Gbrowse``` irá gerar uma URL no github para qualquer objeto que estiver ativo no Vim. Então o Fugitive lhe dá o melhor dos dois mundos.

- **Explorando o history de um repositorio git**
O comando ```:Glog``` é surpreendente. O comportamento padrão deste comando é bastante diferente do comando ```git log```. Considerando que o ```git log``` mostra uma lista e mensagens de commits para o projeto inteiro, o ```:Glog``` carrega todas as revisões anteriores do arquivo atual na lista quickfix. Isto faz com que seja extremamente fácil rever o histórico de um arquivo.

Na sua forma mais básica, você poderá commitar e enviar seu projeto, módulo usando o ```:Gwrite``` para dar stage em seu arquivo, ```:Gcommit -m 'comentário'```, e por fim ```:Gpush``` para enviar seu projeto, módulo, código ao repositório git. Lembrando que é interessante também usar o ```:Gstatus``` para verificar o status de suas ações no git.

> Conhece algum plugin, recurso superior ao Fugitive? show-me!

**Referências, docs do Fugitive:**
<dl>
<dt><a href="http://vimcasts.org/blog/2011/05/the-fugitive-series">VimCasts.org</a></dt>
<br/>
<dt><a href="https://github.com/tpope/vim-fugitive">Fugitive no Github</a></dt>
<br/>
<dt><a href="https://github.com/tpope/vim-fugitive/blob/master/doc/fugitive.txt">Fugitive Doc</a></dt>
<br/>
</dl>

---

###Syntastic
Syntastic é um plugin para o Vim que executa arquivos através de um check sintax externo e exibe os erros para o usuário. Isto pode ser feito por a cada módulo, arquivo salvo ou dinamicamente "enquanto o código é digitado". Se erros de sintaxe forem detectados, o usuário é instanteneamente notificado sem a necessidade de uma compilação ou coisa semelhante.

> O Syntastic é basicamente um checker Cheater de tão bom. Sentirá falta disto em qualquer outro lugar.

As verificações de erros de sintaxe até o momento existe para ActionScript, Ada, AppleScript, Arduíno, AsciiDoc, ASM,BEMHTML, Bro, Bourne Shell,C,C++,C#,Cabal,Chef,CoffeScript,Coco,Coq, CSS, pepino , CUDA, D, Dart, DocBook, Poeira, Elixir, Erlang, eRuby, Fortran, metadados Gentoo, GLSL, Go, Haml, Haskell, Haxe, Guiador, HSS, HTML, Java, JavaScript, JSON, JSX, MENOS, Lex, Limbo, LISP, LLVM linguagem intermediária, Lua, MATLAB, NASM, Objective-C, Objective-C ++, OCaml, Perl, Perl POD, PHP, gettext Portable Object, OS X e iOS listas de propriedades, Puppet, Python, Raquete, R, reStructuredText, Ruby, SASS / SCSS, Scala, Magro, Tcl, TeX, Texinfo, Twig, dactilografados, Vala, Verilog, VHDL, VimL, XHTML, XML, XSLT, YACC, YAML, z80, modelos de página do Zope, e zsh.

Basicamente o Syntastic detecta erros de sintaxe ou de estilo de várias maneiras desde setas apontando o erro, linhas em vermelho, avisos quando o arquivo fora salvo, sinais colocados ao lado de linhas com erros, balão contendo mensagem de erro quando o mouse passa pela linha (no gVim) etc... Ou seja, para linguagens complicadas de encontrar o erro como Java ou C++, este recurso vale ouro.

**Referências, docs do Syntastic:**
<dl>
<dt><a href="https://github.com/scrooloose/syntastic">Syntastic Github</a></dt>
<br/>
<dt><a href="https://github.com/scrooloose/syntastic/blob/master/doc/syntastic.txt">syntastic Doc</a></dt>
<br/>
</dl>

---

###MultiUser

Conhece alguma plataforma de desenvolvimento colaborativo em tempo real? bem, existe o **[Gobby](https://gobby.github.io/)**,o **[Etherpad](https://gobby.github.io/)**, o **[Cloud9](https://c9.io/)**, entre vários outros que permitem este tipo de interação entre os usuários. E algum editor tão poderoso quanto o vim que faz isto? Conhece? Oras, o próprio diria. O MultiUser é um plugin que foi construído para permitir que os usuários de Vim pudessem interagir uns com os outros em tempo real e sobre o mesmo arquivo. O sistema funciona como client/servidor, requer na máquina uma versão superior ou igual ao Python 2.5 instalado, e roda localmente ou através de uma vpn.

Para configurar o servidor, basta instalar o plugin no vim e digitar ```:call MultiUserServer (porta)``` e para o client logar, basta digitar ```:call MultiUserClient ("ip do servidor","porta")```. A porta pode ser a 1337, 2222 ou qualquer outra. Caso deseje criar uma VPN para acesso externo, poderá criar desde OpenVPN a Hamachi tranquilamente.

**Referências, docs do MultiUser:**
<dl>
<dt><a href="https://github.com/emgram769/vim-multiuser">MultiUser Github</a></dt>
<br/>
<dt><a href="https://github.com/emgram769/vim-multiuser/blob/master/doc/vim-multiuser.txt">MultiUser Doc</a></dt>
<br/>
</dl>

---

 
# Instalação e configuração
Caso você seja usuário de GNU/Linux, basta usar o gerenciador de pacotes padrão do seu sistema e instalar o Vim. Por exemplo,uso o Fedora e por padrão, o Fedora usa o YUM. Neste caso seria ```sudo yum install vim```.Caso use o Mac OsX, é recomendável que se baixe o MacVim. No caso do Windows, é recomendável baixar o Vim no **[site oficial](http://www.vim.org/)**. Ainda existem otimizações, configurações que nós usuários costumeiramente compartilhamos na Internet.

Por exemplo, fiz recentemente uma configuração que atende a todas as minhas necessidades dentro do Vim (você também poderá fazer a sua). E para facilitar a instalação e configuração de quem ainda não tem experiência mas que deseja aprender, estudar o VIM, oupara aqueles que já conhecem mas desejam algo já bem moldado, fica a dica : **[https://github.com/lobocode/myvim](https://github.com/lobocode/myvim)**.

Para instalar basta colar estes três comandos em seu console (terminal):  

{% highlight bash %}
$ git clone https://github.com/lobocode/myvim.git
$ cd myvim
$ sudo ./install                    
{% endhighlight %}

> Existem muitos usuários que fazem o mesmo. Caso o modo do qual uso não lhe satisfaça, sinta-se a vontade em buscar uma configuração que supra com as suas necessidades. Ou se preferir, poderá montar sua própria configuração.

# Trabalho social
Não que isto venha a ser importante para você. Mas talvez seja importante para outrem.O Vim é *charity-ware*, isto é, você é incentivado a fazer
doações para órfãos na Uganda através da *[ICCF](http://iccf-holland.org/)* (experimente dentro do VIM executar o comando ```:help uganda```). Ouacessando o site *[Charityware.info](http://charityware.info/)*.

![Vim Uganda](http://www.vim.org/images/vim_drill_small.JPG)

# Complemento
![Tmux](http://www.periplus.com/image/cache/data/6968/9781934356968-300x400.jpg)
Tmux é um multiplexador de terminal. Isto é, ele nos permite usar um único ambiente para lançar vários terminais, ou janelas, cada uma executando o seu próprio processo ou programa. Por exemplo, podemos carregar o Tmux e carregar o editor de texto Vim ao mesmo tempo. A partir disto podemos
 então criar uma nova janela, carregar um console de banco de dados e alternar entre esses programas todos dentro de uma única sessão.

Se você usar um sistema operacional moderno e um terminal que tem abas, isto não pacerá nada prático ou uma novidade relevante. Mas vários programas em execução simultaneamente são apenas uma das características do tmux. Podemos dividir janelas na horizontal ou painéis verticais, que significa que podemos executar dois ou mais programas lado a lado como faríamos no Terminar, algumas wm como i3, xmonad, iterm2 etc.... E podemos fazer isso tudo sem usar o mouse (o que combina e muito com a maneira de se trabalhar com o Vim).

Podemos também nos separar de uma sessão, ou seja, podemos deixar nosso ambiente executado em segundo plano. Se você usou GNU-Screen antes, você provavelmente deve estar familiarizado com esse recurso. Em muitos aspectos, Tmux é como GNU-Screen com um monte de características extras.A diferença é que o Tmux funciona modo client/servidor podendo até trabalhar em pares de maneira remota via ssh.

> A coisa mais impressionante sobre tmux, na minha opinião, é o quão frustrante a auditoria de código era. Em duas horas, eu encontrei apenas um ou dois nits que tiveram conseqüências de segurança muito menores. Ele não foi aceito na árvore com base apenas na licença. É código de alta qualidade. **[Theo de Raadt](http://en.wikipedia.org/wiki/Theo_de_Raadt)**

![Tmux2](https://camo.githubusercontent.com/9a07003e528862ebff782aac2220ef226d28db57/68747470733a2f2f7261772e6769746875622e636f6d2f636872697368756e742f636f6c6f722d736368656d65732f6d61737465722f7468617965722f73637265656e73686f742e706e67)

Além de abrir programas simultaneamente o tmux também permite que a janela seja dividida na horizontal ou vertical, i. e., pode rodar dois programas simultamente na mesma janela, lado a lado, sem falar da capacidade de anexar ou sair de uma sessão sem que ela seja fechada.

A maneira da qual o Tmux funciona para edição em pares, pode parecer redundante já que citei MultiUser "plugin do vim". No entanto, ele te dá a vantagem de ter muito mais controle de janelas e opções de terminal do que o MultiUser propriamente. Ou seja, você conseguirá trabalhar com Vim, bash, sua variações e vários projetos e sessões ao mesmo tempo. A desvantagem em relação ao MultiUser do vim, é que o MultiUser como o próprio nome já sugere, suporta Multi usuários diferentemente do Tmux que tem sua limitação em só trabalhar com usuários na mesma máquina via ssh.Além do que você pode mesclar os dois recursos e aproveitar o melhor de cada. Para saber mais sobre o Tmux com Vim e edição em par, clique **[aqui](https://www.youtube.com/watch?v=ptbLNNNnZXA)**.

# Conclusão 
Embora eu tenha experimentado diversos editores de texto modernos, até a presente data não encontrei nenhum que corresponda a eficiência do Vim. Depois de usar Vim quase todos os dias por tantos anos, ainda estou descobrindo novos recursos, capacidades e comportamentos úteis que melhoram ainda mais a minha produtividade. Vim envelheceu bem ao longo dos últimos 20 anos. Não é apenas uma relíquia, ainda é tão atraente como sempre e continua a atrair novos usuários. A curva de aprendizagem é íngreme, mas os ganhos de produtividade são incríveis e fazem valer muito o esforço em aprende-lo.


**Tutoriais e Dicas do Vim:**
<dl>
<br/>
<dt><a href="http://vimcasts.org/publications/">Pratical Vim</a></dt>
<br/>
<dt><a href="https://code.google.com/p/vimbook/">Vim book- PT-BR</a></dt>
<br/>
<dt><a href="http://www.infowester.com/linuxvi.php">InfoWester</a></dt>
<br/>
<dt><a href="http://aurelio.net/vim/vim-basico.txt">Aurélio - Vim Básico</a></dt>
<br/>
<dt><a href="http://aurelio.net/vim/vim-medio.txt">Aurélio - Vim Médio</a></dt>
<br/>
<dt><a href="http://aurelio.net/vim/vim-avancado.txt">Aurélio - Vim Avançado</a></dt>
<br/>
<dt><a href="https://sites.google.com/site/bemylifeeasy/Home/vimrc">.vimrc - Dicas</a></dt>
<br/>
<dt><a href="http://www.akitaonrails.com/2010/07/19/screencast-comecando-com-vim#.VN623TZGh5Q">Fábio Akita - ScreenCast</a></dt>
<br/>
<dt><a href="http://www.pluralsight.com/courses/smash-into-vim">Smash into Vim</a></dt>
<br/>
<dt><a href="http://vimcasts.org/episodes/">VimCasts.org Screencasts</a></dt>
<br/>
<dt><a href="http://vim.wikia.com/wiki/Tutorial">Vim Wiki</a></dt>
<br/>
<dt><a href="vim-adventures.com">Vim-Adventures</a></dt>
<br/>
<dt><a href="http://code.tutsplus.com/courses/venture-into-vim">Tutplus vim course</a></dt>
<br/>
<dt><a href="https://brizeno.wordpress.com/2014/07/24/por-que-voce-tambem-gostaria-de-utilizar-vim/">Porque você também gostaria de usar Vim?</a></dt>
<br/>
<dt><a href="http://ericdouglas.github.io/2014/03/23/09-motivos-para-aprender-vim/">Motivos para aprender Vim</a></dt>
<br/>
<dt><a href="http://usevim.com/">Use Vim</a></dt>
<br/>
</dl>


