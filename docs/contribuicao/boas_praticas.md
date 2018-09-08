# Boas práticas de programação
***
## 1. Técnicas de programação
***

Programação defensiva é o reconhecimento de que os programas terão problemas e serão modificados

Oferece um conjunto de técnicas para prevenir potenciais problemas de código e tem como objetivo produzir códigos resilientes que respondam adequadamente em situações inesperadas e que seja compreensivel e fácil de dar manutenção

|Técnica|Descrição|
|-------|---------|
|**Estilo e Desing**|Comentarios (linhas, paragrafos, funções e estruturas de controle), nomes de variáveis, métodos e classes significativas|
|**Priorizar a clareza ao inves da concisão**|Tornar o código um livro e sempre priorize a simplicidade do código|
|**Não deixe os outros mexerem onde não devem**|Abuse de encapsulamentos privados ou publicos e etc...|
|**Verifique todos os valores de retorno**|Os testes devem verificar todos os valores possíves de retorno, utilize uma amostragem pequena que engloba praticamente todos os casos|
|**Manipule recursos**|Sempre que abrir um arquivo ou conexão ou etc... feche-o|
|**Inicialize todas as variáveis ao declarar**|Todas as variáveis devem ser inicializadas|
|**Declare as variáveis o mais tarde possível**|Sempre declare elas o mais perto possível de seu uso.|
|**Use sempre recursos padrões da linguagem**|Não reinvente a roda, a menos que seja necessário|
|**Use um sistema de logging**|Abuse dos logs/prints e etc...|
|**Siga o idioma da linguagem**|Códifique em inglês sempre.|
|**Verifique os limites númericos**|Faça um código defensivo que não quebre em um determinado limite númerico|
|**Use constantes**|Acabe com os números mágicos|
|**Decomposição em funções atômicas**|Sempre deixe as funções com o minimo de código possivel realizando apenas o que ela deve realizar.|
|**Utilize paragrafos de função**|Dentro de uma função separe-a em paragrafos|
|**Utilize tipagem**|Se a linguagem for de tipagem dinâmica tente arranjar um jeito de fazer o usuário usar somente o tipo desejado com código defensivo, exceções por exemplo.|
|**Cabeçalhos e docstring**|Documente seu código|
|**Tratamente de erros apropriados**|Trate os erros em nível apropriados usando exceptions|
|**Assertivas**|Use em partes do código em que o erro não pode ser permitido, tendo que fechar a aplicação caso ocorra.|
|**Assuma o pior**|Sempre assuma que o pior pode acontecer no seu código e prepare-o para suportar esses eventos.|

***
## 2. Comentários e Docstring
***

Sempre tenha como prioridade manter os comentários atualizados com as mudanças no código, e sempre comente em ingles!

#### Comentar linha individual

- Quando a linha de código é extremamente complicada e não há como simplificar
- Quando registrar um erro já ocorrido em uma linha

#### Comentar paragrafo de código

- No máximo duas linhas e escreve o por que em vez de como,
- Utilize o comentário para preparar o leitor para o que vem a seguir,
- Se for por motivo de performace, deixe claro o beneficio

#### Comentar declaração de variáveis

- Descrever aspectos da variável que o nome não consegue representar,
- Por exemplo, unidade de medida, o intervalo permitido para valores númericos, documentar variáveis globais
- Devem ser separados da variável por pelo menos dois espaços.

#### Comentar estruturas de controle

- Para estruturas de decisão como if e case, pode-se comentar o motivo da decisão e um resumo do resultado obtido,
- No caso de loops, pode ser indicado o seu propósito, inclua sempre antes da estrutura de controle

#### Docstrings

- Escreva docstrings para todo módulo, função, classe e método público.
- Elas não são necessárias para métodos "privados", mas é recomendável ter um comentário que explique o que ele faz.
- Este comentário deve estar logo após a declaração do método privado.

***
## 3. SOLID
***

#### Alta coesão

É fator de qualidade de projeto e representa que cada classe tem sua respectiva responsabilidade bem definida

#### Baixo acoplamento

É fator de qualidade em um projeto que busca a medida de interdependência entre modulos, modulos com baixo acoplamento são mais independentes.

#### Single responsability principle

Cada classe/metodo devem ter responsabilidades únicas, logo uma classe Conta não é responsavel por fazer transferencias, ela deve designar essa responsabilidade a classe de fazer transferencias, tornando as classe mais coesas.

#### Open-closed principle

Uma classe deve ser aberta a extensão (herança) e fechadas a modificações, é basicamente deixar sua classe ser extensivel, por exemplo, crio a classe Carro e crio várias outras classe que herdam de carro para extender essa classe, por exemplo, CarroSedan, CarroPopular, CarroQuebrado, CarroFeio, e etc... cada um responsavel por suas modificações.

#### Liskov substitution principle

O cliente deve usar o serviço da classe abstrata (geral) sem saber que ta usando um serviço especifico concreto, por exemplo temos a classe Carro abstrata e as classes concretas Gol e Palio que herdam dessa abstrata, o cliente pode usar o Carro sem saber se o carro é um Gol ou um Palio, isso é mais usado em linguagens com tipagem estática que não é o caso do python.

#### Interface segregation principle

Uma interface não deve obrigar quem a implementar a implementar métodos que não agrega valor a ela, por exemplo, a classe Mamifero tem os métodos que deve ser implementado por Pessoa e Cachorro que são mamiferos, andar e falar, porém cachorro não fala, logo ele não deve ser obrigado a implementar esse método, ele deve criar seu método latir

#### Dependency Inversion Principle

Uma classe deve depender de classes abstratas/interface e não de suas classes concretas que ta a implementação, é basicamente igual ao Liskov substitution, porém voltado a dependencia uma frabrica de carros deve depender da classe abstrata Carro e não das concretas Gol ou Palio.

***
## 5. Testes
***

**Teste**: processo de detectar o erro inicial

* Para rodar os testes execute: ```make test```

* Para roda o coverage: ```make report```

* Para roda o coverage em html: ```make html```
