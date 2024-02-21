<h1 id="title"> Como nomear seus commits de forma simples </h1>

<p align="center" id="badges">
    <img loading="lazy" src="http://img.shields.io/static/v1?label=STATUS&message=EM%20DESENVOLVIMENTO&color=GREEN&style=for-the-badge" alt="Status Badge"/>
</p>

🚀 Doc simples para entender como, quando e por que utilizar os *"Conventional Commits"* em nossos commits de forma simples e simplificada

<h3 id="indice">Índice</h3>

* [Título e Imagem de capa](#title)
* [Badges](#badges)
* [Índice](#indice)
* [Introdução](#intro)
* [Tipos mais comuns](#types)
* [Deixando os commits mais "bonitos"](#beauty-commits)
* [Principais Regras de uso](#main-rules)
* [Como descrever um commit?](#how-to-describe)
* [Conclusão](#conclusion)
* [Referências](#references)

<h3 id="intro">Introdução</h3>

Assim como eu, você já deve ter se perguntados várias vezes :question: :  
*"Beleza, fiz tudo o que eu tinha que fazer :white_check_mark: , mas como eu vou nomear esse commit para que os outros entendam o que eu fiz?"*

Para tentar responder, eu sempre pensei na base da pergunta: **"PARA OS OUTROS"**
Isso significa que o principal papel de um commit **bem descritivo** é **facilitar** o papel da **próxima pessoa** no nosso projeto. :smile:
Imagine receber uma nova task de continuidade ao processo criativo iniciado por outra pessoa e o último commit no repositório é:  
*"Fix some bugs"* :fearful:  

Não sei você, mas ia ficar perdidinho procurando no código o que foi corrigido ou não, com uma grande chance de deixar algo passar, simplesmente pelo motivo de não saber o que foi feito no commit!!

Então resolvi fazer essa pequena doc para aumentar a eficácia do entendimento dos nossos commits e evoluir nossa produtividade :rocket::rocket::rocket:

<h3 id="types">Tipos mais comuns</h3>

No mundo dev temos várias formar de entitular e descrever nossos commits, dentre todas essas formas eu escolhi trazer de forma resumida os **"Conventional Commits"**  

De forma resumida os **"Conventional Commits"** são simples prefixos para identificar os tipos de mudanças feitas no código.
O objetivo de cada um desses prefixos é organizar o tipo de mudança feita naquele commit afim de ser útil para todos os devs que participam do projeto.

<h4>Tipos</h4>

* **`feat:`** Um commit que adiciona ou remove uma nova feature
**Exemplo:** Uma função totalmente nova da aplicação ou sua remoção  

* **`refactor:`** Uma refatoração feita no código que não vai alterar em nada a funcionabilidade ou qualquer tipo de lógica nas regras de negócio do projeto
**Exemplo:** Alterar uma função "grande" para uma forma menos verbosa.

* **`style:`** Nesse caso podemos usar para duas situações:
**1º - (Front-End)** Alterações exclusivas na folha de estilo da aplicação
**Exemplo:** Alterações no estilo da página, geralmente nos arquivos de estilos (CSS, SASS, LESS, Styled-Componentes...)
**2º** Mudanças na formatação do código que não alteram nenhuma regra de negócio
**Exemplo:** Alterações nos formatadores, configurações nas convenções de *lint*, remover comentários, espaços em branco, etc...

* **`fix:`** A correção de algum problema/erro/bug no código
**Exemplo:** Criar uma validação no uso de algum elemento da DOM para tratar o erro quando esse elemento não existir.

* **`chore:`** Mudanças na forma de compilar o projeto, adição de novos arquivos de configuração ou até mesmo ao adicionar novas bibliotecas.
**Exemplo:** Adicionar um arquivo *``.gitignore``*.

* **`docs:`** Esse é simples (UFA), usado para indicar mudanças na documentação do projeto.
**Exemplo:** Alteras essa linda DOC que você está lendo agora!! :dizzy:

* **`build:`** Alterações no processo de *BUILD* ou nas dependências do projeto.
**Exemplo:** Mudanças no ``GULP`` ou remover/adicionar dependencias no ``yarn``.

* **`perf:`** Alterações específicas para melhorar a perfomace da aplicação.
**Exemplo:** Trocar um *map()* por um *forEach()*

* **`revert:`** Destaca uma *reversão* diretamente relacionada ao *commit* anterior.
**Exemplo:** Aqui não precisamos de exemplo (Assim espero :warning:).

```git
    git commit -m "feat: add buy together module"
    git commit -m "refactor: change way to loop for users"
    git commit -m "style: responsive styles for user card"
    git commit -m "fix: bug of duplicated users"
    git commit -m "chore: add .gitignore file"
    git commit -m "docs: add new commit patterns section"
    git commit -m "build: remove example.js dependency"
    git commit -m "perf: remove an unnecessary loop"
    git commit -m "revert: back to a862956 commit"
```

<span style="font-size:0.7rem;">Exemplos dos tipos de commit citados anteriormente</span>

<h3 id="beauty-commits">Deixando os commits mais "bonitos"</h3>

Vamos deixar as coisas mais bonitas, organizadas e de fácil visualização:
<h4>Padrões de Emoji</h4>
<table>
  <thead>
    <tr>
      <th>Tipo do commit</th>
      <th>Emoji</th>
      <th>Palavra-chave</th>
    </tr>
  </thead>
 <tbody>
    <tr>
      <td>Adicionando uma dependência</td>
      <td>➕ <code>:heavy_plus_sign:</code></td>
      <td><code>build</code></td>
    </tr>
    <tr>
      <td>Alterações de revisão de código</td>
      <td>👌 <code>:ok_hand:</code></td>
      <td><code>style</code></td>
    </tr>
    <tr>
      <td>Animações e transições</td>
      <td>💫 <code>:dizzy:</code></td>
      <td><code>style</code></td>
    </tr>
    <tr>
      <td>Bugfix</td>
      <td>🐛 <code>:bug:</code></td>
      <td><code>fix</code></td>
    </tr>
    <tr>
      <td>Comentários</td>
      <td>💡 <code>:bulb:</code></td>
      <td><code>docs</code></td>
    </tr>
    <tr>
      <td>Commit inicial</td>
      <td>🎉 <code>:tada:</code></td>
      <td><code>chore</code></td>
    </tr>
    <tr>
      <td>Configuração</td>
      <td>🔧 <code>:wrench:</code></td>
      <td><code>chore</code></td>
    </tr>
    <tr>
      <td>Deploy</td>
      <td>🚀 <code>:rocket:</code></td>
      <td><code>feat</code></td>
    </tr>
    <tr>
      <td>Documentação</td>
      <td>📚 <code>:books:</code></td>
      <td><code>docs</code></td>
    </tr>
    <tr>
      <td>Em progresso</td>
      <td>🚧 <code>:construction:</code></td>
      <td><code>feat</code></td>
    </tr>
    <tr>
      <td>Mover/Renomear</td>
      <td>🚚 <code>:truck:</code></td>
      <td><code>chore</code></td>
    </tr>
    <tr>
      <td>Novo recurso</td>
      <td>✨ <code>:sparkles:</code></td>
      <td><code>feat</code></td>
    </tr>
    <tr>
      <td>Package.json em JS</td>
      <td>📦 <code>:package:</code></td>
      <td><code>build</code></td>
    </tr>
    <tr>
      <td>Performance</td>
      <td>⚡ <code>:zap:</code></td>
      <td><code>perf</code></td>
    </tr>
    <tr>
        <td>Refatoração</td>
        <td>♻️ <code>:recycle:</code></td>
        <td><code>refactor</code></td>
    </tr>
    <tr>
      <td>Removendo um arquivo</td>
      <td>🔥 <code>:fire:</code></td>
      <td><code>chore</code></td>
    </tr>
    <tr>
      <td>Removendo uma dependência</td>
      <td>➖ <code>:heavy_minus_sign:</code></td>
      <td><code>build</code></td>
    </tr>
    <tr>
      <td>Responsividade</td>
      <td>📱 <code>:iphone:</code></td>
      <td><code>style</code></td>
    </tr>
    <tr>
      <td>Estilização</td>
      <td>💄 <code>:lipstick:</code></td>
      <td><code>style</code></td>
    </tr>
    <tr>
      <td>Revertendo mudanças</td>
      <td>💥 <code>:boom:</code></td>
      <td><code>fix</code></td>
    </tr>
    <tr>
      <td>SEO</td>
      <td>🔍️ <code>:mag:</code></td>
      <td><code>refactor</code></td>
    </tr>
    <!-- <tr>
      <td>Testes</td>
      <td>🧪 <code>:test_tube:</code></td>
      <td><code>test</code></td>
    </tr> -->
    <tr>
      <td>Tratamento de erros</td>
      <td>🥅 <code>:goal_net:</code></td>
      <td><code>fix</code></td>
    </tr>
  </tbody>
</table>

<h4>Exemplos</h4>
<table>
  <thead>
    <tr>
      <th>Comando Git</th>
      <th>Resultado no GitHub</th>
    </tr>
  </thead>
 <tbody>
    <tr>
      <td>
        <code>git commit -m ":tada: Commit inicial"</code>
      </td>
      <td>🎉 Commit inicial</td>
    </tr>
    <tr>
      <td>
        <code>git commit -m ":books: docs: seção de como commitar"</code>
      </td>
      <td>📚 docs: Seção de como commitar</td>
    </tr>
    <tr>
      <td>
        <code>git commit -m ":bug: fix: Reatribuição de const"</code>
      </td>
      <td>🐛 fix: Reatribuição de const</td>
    </tr>
    <tr>
      <td>
        <code>git commit -m ":sparkles: feat: Módulo de compre junto"</code>
      </td>
      <td>✨ feat: Módulo de compre junto</td>
    </tr>
    <tr>
      <td>
        <code>git commit -m ":recycle: refactor: Passa para forEach()"</code>
      </td>
      <td>♻️ refactor: Passa para forEach()</td>
    </tr>
    <tr>
      <td>
        <code>git commit -m ":zap: perf: Altera o tamanho renderizado das imagens"</code>
      </td>
      <td>⚡ perf: Altera o tamanho renderizado das imagens</td>
    </tr>
    <tr>
      <td>
        <code>git commit -m ":lipstick: feat: Estilização CSS do formulário"</code>
      </td>
      <td>💄 feat: Estilização CSS do formulário</td>
    </tr>
    <tr>
      <td>
        <code>git commit -m ":bulb: docs: Comentários sobre a função addToCart( )"</code>
      </td>
      <td>💡 docs: Comentários sobre a função addToCart( )</td>
    </tr>
  </tbody>
</table>

<h3 id="main-rules">Principais Regras de uso</h3>

* Só pode ser utilizado um *type* por commit
* O *type* é obrigatório em todo e qualquer commit

<h3 id="how-to-describe">Como descrever um commit?</h3>

Depois de aprender e entender os casos de uso de cada tipo de commit você deve estar se perguntando:  
*"Hmm, mas eu sou péssimo em descrever o que eu fiz, foi tanta coisa que nem sei por onde começar"*

E é exatamente por ler a sua mente que vou deixar algumas dicas aqui:  

* **Seja imperativo:** Sempre pense que seu commit deve completar essa frase: *"Esse commit irá {Descrição do commit aqui}*  
**Exemplo:** Se você criou um módulo de compre junto completo, você pode pensar *"Esse commit irá adicionar o módulo de compre junto"* o resultado seria  

    ```git
    git commit -m "feat: add buy together module"
    ```

* **Não crie um commit infinito:** é comum abordar diversas tarefas em um único commit, afinal você já esta com a mão na massa :wrench:, mas isso vai dificultar muito a organização dos commits e na descrição também, portanto, prefira *commitar* com mais frequência e particionar suas tarefas pensando nos tipos que mencionamos aqui, sem acumular vários tipos de commits em um só!

* **Indeciso?:** Se você ficou em dúvida sobre qual *type* deve usar no seu commit, muito provavelmente seu commit abordou muitas mudanças e está na hora de pensar em dividir esses commits hein!?

<h3 id="conclusion">Conclusão</h3>

Legal né?  
Achou difícil?

* [x] Claro que não, facinho
* [ ] Muita informação :skull::skull:
* [ ] Mó fome

É claro que não é do dia pra noite que nossos commits ficam lindos e de fácil entendimento, mas tenho certeza de que essas dicas irão de ajudar a ser mais claro e objeto na hora de commitar para facilitar a comunicação na sua equipe!! :heart:

<h3 id="references">Referências</h3>

* <https://medium.com/linkapi-solutions/conventional-commits-pattern-3778d1a1e657>
* <https://blog.rocketseat.com.br/como-fazer-um-commit-conventional-commits/>
* <https://github.com/iuricode/padroes-de-commits/blob/main/README.md>
* <https://www.alura.com.br/artigos/simplificando-controle-versao-conventional-commits>
* <https://www.conventionalcommits.org/pt-br/v1.0.0/>
