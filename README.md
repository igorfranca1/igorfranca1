---
id: comandos_visao
title: Comandos utilizados pela visão
description: Aqui serão explicados quais são os comandos da visão e suas funções
slug: /cmd_visao
sidebar_position: 2
---

A visão utiliza basicamente dois comandos que habilitam o seu funcionamento, sendo eles:


```py
roslaunch object_finder vision.launch
```
O _roslaunch_ é um comando que __começa__ ou __para__ um _node (Processo que realizada computação) ROS_ que leva um ou mais arquivos tipo _.launch_ como argumentos. Para usar o launch é necessário o nome do arquivo tipo _launch_. Você pode especificar o caminho ou o arquivo _launch_ ou você pode especificar o nome do pacote e o arquivo _launch_ dentro desse pacote (como fazemos).

```py
roslaunch <nome_do_pacote> <arquivo_.launch>
```

No nosso caso, executamos o vision.launch dentro do pacote _objectfinder_.

Esse comando inicia todos os códigos da visão, além de poder receber alguns argumentos, sendo eles:

**camera** : Recebe qual a câmera será utilizada (default 0).

**img_output** : Recebe um booleano (true ou false) se terá um retorno visual (default = false).

**ajuste** : Recebe um booleano para entrar no modo de ajuste de brilho, onde será utilizado "=" para aumentar o brilho, "-" para diminuir e "w" para continuar detecção (default = false).

**brilho** : Recebe um valor entre -64 e 64 para o fator de brilho da câmera (default = 4).

```py
rosrun object_finder connecting_and_showing.py
```

O _rosrun_ permite você executar um arquivo executável dentro de um pacote arbitrário de qualquer lugar sem ter que digitar seu caminho completo ou _cd/roscd_ primeiro.

```py
rosrun <pacote> <executavel>
```
Neste caso, executamos o arquivo __Python__ _connect_and_showing.py_ dentro do diretorio _object_finder_.

É o comando que roda o código do connecting and showing, que executa as funções da visão no geral

:::tip Como passar o argumento

Utilizar o modelo "nome_argumento:=valor_desejado"

:::

# __VISÃO__ <h1>

A __VISÃO__ na __EDROM__ é responsável pela visão computacional dos robôs desenvolvidos pela __EDROM__. A _Visão Computacional_ é responsável pelo funcionamento, reconhecimento e tratamento das imagens recebidas pela câmera dos robôs.

A __VISÃO__ também é responsável pela criação de amostras e treinamento de rotulação de objetos em imagens, processo também conhecido como image labelling que consiste na identificação e marcação de um determinado objeto em uma imagem e atribuindo um valor (ou nome) para ele. Esse processo é feito pela equipe da __VISÃO__ e em seguida é executado o programa de treinamento de aprendizado de _rede neural_ que será encarregado de detectar e decifrar padrões e correlações, do mesmo jeito que os humanos aprendem e raciocinam.

A principal linguagem de programação usada na __VISÃO__ é __Python__, onde temos aplicações que auxiliam no tratamento de arquivos de texto e imagens para os treinamentos, devido a sua facilidade no acesso e manipulção de repositórios. A principal biblioteca de __Python__ utilizada para o desenvolvimento dos nossos aplicativos de __Visão__ Computacional é a _OpenCV (sigla para Open Source Computer Vision Library)_ que é responsável pelo _Processamento de Imagens e Entrada e Saida de Video_, dentre outras funções.



<!--
**igorfranca1/igorfranca1** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

