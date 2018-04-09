# Git

*Alguns exercícios nesta secção assumem o uso de Visual Studio 2017 com a
extensão "Git for Windows".*

1 - Quando crias um novo projeto em Visual Studio 2017 com repositório Git
inicializado, que comandos Git são executados automaticamente em pano de fundo?

> [Soluções](../solucoes/01_git/01.md)

---

2 - Como podes, dentro do Visual Studio 2017, inicializar um repositório Git
num projeto já existente (criado sem repositório Git)? E usando o terminal?

> [Soluções](../solucoes/01_git/02.md)

---

3 - Para que serve o ficheiro `.gitignore`? Explica o porquê deste ficheiro
ser essencial num projeto em Visual Studio?

> [Soluções](../solucoes/01_git/03.md)

---

4 - Para que serve o ficheiro `.gitattributes`?

> [Soluções](../solucoes/01_git/04.md)

---

5 - O Git é especialmente adequado para controlar as versões de que tipo de
ficheiros? Por outro lado, que tipo de ficheiros não é recomendável adicionar a
um repositório Git? Explica como essa limitação poderia à partida "atrapalhar"
o desenvolvimento de vídeo jogos?

> [Soluções](../solucoes/01_git/05.md)

---

6 - Quais são os comandos Git para especificares, de uma forma global, o teu
**nome** e **email** para realização de *commits*? E caso queiras efetuar essa
configuração apenas para um repositório?

> [Soluções](../solucoes/01_git/06.md)

---

7 - Apresenta os conteúdos do ficheiro `.gitignore` quando pretendes evitar que
os ficheiros com extensão `.exe`, `.dll`, `.jpg` e `.png` sejam adicionados ao
repositório.

> [Soluções](../solucoes/01_git/07.md)

---

8 - Escreve os comandos git para: 1) adicionar um repositório remoto chamado
_origin_ com URL https://github.com/VideojogosLusofona/BestGameEver; 2) fazer
_push_ do ramo local _master_, com seguimento, para o repositório remoto
_origin_ adicionado no ponto anterior.

> [Soluções](../solucoes/01_git/08.md)

---

9 - Na sequência do exercício anterior, qual o comando git para alterar o nome
do repositório conhecido como _origin_ para _secondary_? E se quiséssemos
apenas mudar o URL para https://github.com/VideojogosLusofona/not-so-good-game?

> [Soluções](../solucoes/01_git/09.md)

---

10 - Escreve os comandos git para: 1) alterar o nome do ficheiro `Programa.cs`
para `Jogo.cs`; 2) fazer _commit_ da alteração efetuada, com uma mensagem de
_commit_ que siga as [melhores práticas](https://gist.github.com/robertpainsi/b632364184e70900af4ab688decf6f53)
para o efeito.

> [Soluções](../solucoes/01_git/10.md)

---

11 - Fizeste modificações aos ficheiros `README.md` e `MyGame/Program.cs`, e
queres realizar um _commit_ com a mensagem "Update documentation and comments".
Quais os comandos necessários para realizar este _commit_?

> [Soluções](../solucoes/01_git/11.md)

---

12 - Estás a trabalhar no ramo `experiment`, e decides que a alteração
experimental que fizeste é suficientemente boa para juntar ao ramo principal do
programa (`master`). Qual o comando ou comandos para o efeito?

> [Soluções](../solucoes/01_git/12.md)

---

13 - Qual o comando para ver as diferenças entre o penúltimo _commit_ e o
antepenúltimo _commit_? Podes assumir que estamos num ramo sem divergências,
ou seja, cada _commit_ tem apenas um pai.

> [Soluções](../solucoes/01_git/13.md)

---

14 - Por engano adicionaste uma pasta de nome `bin`, bem como todos os seus
conteúdos, para _commit_ (isto é, à _staging area_). No entanto, ainda não
fizeste _commit_. Qual o comando para retirar essa pasta, bem como os seus
conteúdos, da _staging area_?

> [Soluções](../solucoes/01_git/14.md)

---

15 - Qual o comando para descartar todas as alterações efectuadas em ficheiros
Markdown (extensão `.md`) ainda não adicionadas para _commit_ (isto é, ainda
não adicionadas à _staging area_)?

> [Soluções](../solucoes/01_git/15.md)

---

16 - Qual a diferença entre um _merge fast forward_ e um _merge commit_? Em
qual destes _merges_ é possível haver um _merge conflict_?

> [Soluções](../solucoes/01_git/16.md)

---

17 - Escreve os comandos git para o teu repositório ficar com um estado
semelhante ao indicado na imagem em baixo. Não te esqueças que é necessário
existirem alterações na _staging area_ de modo a ser possível fazer um
_commit_, pelo que deves indicar também estas modificações (os nomes de
ficheiros podem ser inventados por ti).

![git01](https://user-images.githubusercontent.com/3018963/37652984-3b37d760-2c35-11e8-9ad2-9461c87fccf0.png)

> [Soluções](../solucoes/01_git/17.md)

---

18 - Apagaste o ramo `new-feature` do teu repositório local, ramo esse que
estava também mapeado (com o mesmo nome) no repositório remoto `upstream`. Qual
é o comando para apagar o ramo também no repositório remoto?

> [Soluções](../solucoes/01_git/18.md)

---

19 - Estás a trabalhar no teu projeto final de LP1, e tens alguns _commits_ no
ramo `devel` que ainda não foram sincronizados com o teu servidor remoto
(conhecido localmente como `upstream`). Qual o comando para realizar esta
sincronização/carregamento de alterações com o servidor remoto?

> [Soluções](../solucoes/01_git/19.md)

---

20 - Estás a trabalhar com o teu colega no projeto final de LP1, e o teu colega
criou alguns ramos e fez _push_ de algumas alterações no servidor remoto
(localmente conhecido como `mygithub`). Qual o comando para o teu repositório
local ficar com conhecimento sobre todas as alterações efectuadas no
repositório remoto (incluindo novos ramos)?

> [Soluções](../solucoes/01_git/20.md)

---

21 - Estás a trabalhar no ramo local `master`, e tens alguns _commits_ feitos
desde a última vez que sincronizaste com o remoto `origin`. Ao fazeres `push`
das tuas alterações, obténs a seguinte mensagem:

```
error: failed to push some refs to 'https://gitlab.com/ulht/projeto.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
```

Explica qual é o problema e como o podes resolver, assumindo que não existem
_merge conflicts_.

> [Soluções](../solucoes/01_git/21.md)

---

22 - Estás a trabalhar no ramo local `master`, e tens alguns _commits_ feitos
desde a última vez que sincronizaste com o remoto `origin`. Antes de fazeres
o `push` dos teus _commits_ locais, tentas integrar possíveis _commits_ em
`origin/master` no teu `master` local (fazendo por exemplo, `git pull`), mas
obténs a seguinte mensagem de erro:

```
Unpacking objects: 100% (6/6), done.
From https://gitlab.com/ulht/projeto.git
   17858a5..1601016  master     -> origin/master
Auto-merging MyGame/BigBadBoss.cs
CONFLICT (content): Merge conflict in MyGame/BigBadBoss.cs
Automatic merge failed; fix conflicts and then commit the result.
```

Explica qual é o problema e como o podes resolver.

> [Soluções](../solucoes/01_git/22.md)

---

23 - Como podes eliminar localmente o conhecimento sobre o remoto chamado
`origin`?

> [Soluções](../solucoes/01_git/23.md)

---

24 - Estás a trabalhar há algum tempo num repositório local, mas decidiste que
seria importante ter um repositório remoto para _backup_ e possíveis
colaborações com terceiros. Criaste o repositório remoto no GitLab no URL
https://gitlab.com/MyUsername/bestgamever.git, e agora pretendes associar este
remoto ao teu repositório local com o nome `principal` e fazer `push` do ramo
local `master` para o ramo remoto `master`. Além disso queres tornar o ramo
`master` local num _remote tracking branch_ (ramo de seguimento remoto) do
ramo `principal/master`. Quais são os comandos para alcançares estes objetivos?

> [Soluções](../solucoes/01_git/24.md)
---

25 - Chegaste à conclusão que o nome `principal` não é apropriado para o
repositório remoto do exercício anterior. Qual o comando para mudares o nome
do remoto para `origin`?

> [Soluções](../solucoes/01_git/25.md)

---

26 - Explica por palavras tuas o que é um _remote tracking branch_ (ramo de
seguimento remoto)?

> [Soluções](../solucoes/01_git/26.md)

---

27 - Como podes obter localmente informação detalhada sobre um remoto conhecido
como  `upstream`?

> [Soluções](../solucoes/01_git/27.md)

---

28 - Como podes obter informação detalhada sobre um ramo local chamado `devel`,
incluíndo a sua associação de seguimento remoto com um potencial ramo remoto?

> [Soluções](../solucoes/01_git/28.md)

---

29 - Tens um ramo local chamado `testing` e queres fazer `push` desse ramo para
o remoto localmente conhecido como `main`. No entanto o remoto em questão já
tem um ramo com esse nome. Como podes fazer `push` (com seguimento) do teu ramo
local `testing` de modo a que este seja conhecido remotamente como `mytesting`?

> [Soluções](../solucoes/01_git/29.md)

---

30 - Tens um ramo local chamado `new-level` e queres que este ramo passe a
fazer _remote tracking_ (seguimento) do ramo `devel` no remoto localmente
conhecido como `origin`. Qual é o comando para o efeito?

> [Soluções](../solucoes/01_git/30.md)

---

31 - O teu repositório local tem conhecimento de dois remotos: `origin` e
`upstream`. Existe um ramo chamado `new-boss` no remoto `origin`, que não
existe localmente nem no remoto `upstream`. Quais os comandos para passares a
ter este ramo localmente e no remoto `upstream`, com o mesmo nome? Certifica-te
que o ramo `new-boss` local não faz seguimento a nenhum ramo remoto.

> [Soluções](../solucoes/01_git/31.md)

---
