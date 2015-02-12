---
layout: post
title: Vim é o poder
snip:  IDE pra quê? 
---

O Vim é um editor de texto extremamente configurável, criado para permitir a edição de textos de forma eficiente. Também é um melhoramento do editor vi, um tradicional programa dos sistemas UNIX. Possui uma série de mudanças em relação a este último. O próprio slogan do vim é "Vi IMproved". Ou seja, Vi Melhorado. O Vim é tão conhecido e respeitado entre programadores, e tão útil para programação, que muitos o consideram uma verdadeira IDE. Ele é capaz de reconhecer mais de 400 sintaxes de linguagens de programação e marcação, possui mapeamento para teclas, macros, abreviações, busca por expressões regulares, entre outras facilidades. Conta com uma comunidade bastante atuante e é, ao lado do GNU Emacs um dos editores mais usados nos sistemas GNU, mas pode ser também instalado em outros sistemas, como o Windows e o Mac e BSD.

## Editores modernos ##

Vivemos em um tempo em que há uma grande variedade de editores que são usados para inúmeros fins. Como é o caso do Atom [https://atom.io]. Este é um editor que foi fortemente baseado no SublimeText [www.sublimetext.com] e que por muitos, já é considerado o melhor editor para desenvolvedores. Ao observar este quadro, vem em mente uma primeira preocupação: longevidade. Parece que passamos uma grande quantidade de tempo nos comprometendo com teclas atalhos, manuais, tutoriais para aprender a manuzear recursos que são específicos para o que estamos usando em um determinado editor e ao mesmo tempo, nos perdendo com a variedade absurda de ferramentas oferecidas nos mais variados editores. Tanto o Atom, quanto o SublimeText, por exemplo, misturam uma interface gráfica ao lado de uma necessidade de codificação simples. Esta necessidade, na verdade, surgiu como alternativa a editores pesados como é o caso do Adobe DreamWeaver ( largamente usado na década de 90 e por algumas pessoas ainda hoje ). Ou algo como o Eclipse que pode incluir tudo o que você possa imaginar...talvez até algo como... uma pia de cozinha!?

O fato é, nem Sublime, nem Atom, são tão leves e "onipresentes" quanto o VIM. Basicamente, o VIM está disponível por padrão até em sistemas operacionais mais antigos e pode rodar em todos os sistemas que podem implementar a biblioteca C padrão "ou o VI que muda somente alguns comandos" mas que carrega a mesma essência. O grande problema com o uso de IDEs pesadas como Eclipse ou Netbeans, é que geralmente você não pode manipular ou escolher exatamente que tipo de recurso que deseja usar ou deixar de usar neles. IDEs tem a vantagem de serem capazes de atingir uma plataforma ou linguagem específica ( como por exemplo, o Java, PHP ou Android ). Ou seja, a IDE pode fornecer mais controle comparado a um editor de texto que é reforçado com recursos variados. 

Já imaginou trabalhar em um editor que pode ser moldado a todas as suas necessidades como desenvolvedor? bem, o VIM oferece esta proposta. Por padrão, o VIM vem igual para todos os usuários. Exceto quando você resolve modificar o seu .vimrc file. Ou seja, existe um arquivo com suas próprias configurações ( seja alguma mudança de hotkey "tecla atalho", configuração de comportamento do software mediante uma necessidade específica, plugins, funções que irão ser exercidas em um determinado momento do código, modelos e padrões estabelecidos por você). Além disso, ao meu ver, tem também a grande vantagem de rodar muito leve em qualquer máquina ( até as mais antigas ou em servidores que não contém servidor gráfico rodando).

## Instalação e configuração ##

ralmente o VI vem por padrão em diversos sistemas como o antigo AmigaOS, GNU Hurd, GNU/Linux, BSD, Osx, IRIX, o antigo BeOS,AIX, sistemas POSIX em geral ou qualquer um que rode a biblioteca C padrão. Ou seja, sua instalação não é necessária em muitos casos havendo apenas a necessidade de instalar sua versão melhorada "o VIM". Para tal, basta apenas setar o comando correspondente ao seu gerenciador de pacotes e instalar o VIM. Além disso, existem personalizações que nós usuários costumeiramente compartilhamos na Internet. Por exemplo, fiz recentemente uma configuração pessoal do meu vim para que possar ser baixado e configurado a qualquer lugar que for. E para facilitar a instalação e configuração de quem ainda não tem experiência mas que deseja aprender, estudar o VIM, fica a dica :[https://github.com/lobocode/myvim].

Para instalar basta colar estes três comandos em seu console (terminal):  

{% highlight bash %}
$ git clone https://github.com/lobocode/myvim.git
$ cd myvim
$ sudo ./install                    
{% endhighlight %}


