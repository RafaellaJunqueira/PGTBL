# Introspecção

## 1. Introdução
A técnica de introspecção se baseia em imaginar que tipo de sistema seria utilizado ao executar determinada tarefa, utilizando este equipamento, entre outros. Ou
seja, calcular as propriedades que o sistema deve possuir para que atenda as necessidades do seu público.
***
## 2. Objetivo
Este documento tem por finalidade apresentar os requisitos funcionais elicitados pela técnica de introspecção.
***
## 3. Metodologia
O analista de requisitos busca por histórias de usuário baseadas no que ele imagina que os usuarios do sistema precisam que seja fornecido pelo software separando tais necessidades por prioridades (MoSCoW).
***
## 4. Introspecção
<b>Personas</b><br>
À partir de uma visão geral do produto e à fim de propor situações diferentes do previsto em um cenário comum de possibilidades, as personas aparecerem para se relacionarem com algum tipo de envolvimento, no contexto de requisitos, com o PGTBL, sendo esse contato direto ou não. A prioridade MoSCoW também será determinada de acordo com as necessidades da persona em questão.

Exemplo de situações "comuns"
<table role="table">
<thead>
<tr>
<th align="left">ID</th>
<th align="left">Requisito</th>
<th align="left">Prioridade</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left"><code>1</code></td>
<td align="left">Deve ser possível gerenciar as aulas através do TBL</td>
<td align="left">Must</td>
</tr>
<tr>
<td align="left"><code>2</code></td>
<td align="left">Deve ser possível qualificar os alunos para o mercado de trabalho</td>
<td align="left">Must</td>
</tr>
<tr>
<td align="left"><code>3</code></td>
<td align="left">Deve ser possível aos professores e alunos alterar dados cadastrais</td>
<td align="left">Should</td>
</tr>
<tr>
<td align="left"><code>3</code></td>
<td align="left">Deve ser possível aos professores administrar suas disciplinas e seus alunos</td>
<td align="left">Should</td>
</tr>
 <tr>
<td align="left"><code>4</code></td>
<td align="left">Deve ser possível aos professores visualizar relatório dos alunos e realizar feedback</td>
<td align="left">Should</td>
</tr>
</tbody>
</table>

<h4 id="persona-1-fganderon">Persona 1 - Caroline</h4>
<table>
<thead>
<tr>
<th><strong>Persona 1 </strong></th>
<th><strong>Caroline</strong></th>
</tr>
</thead>
<tbody>
<tr>
<td><strong>Nome:</strong></td>
<td>Caroline</td>
</tr>
<tr>
<td><strong>Profissão:</strong></td>
<td>Estudante de Comunicação da UnB</td>
</tr>
<tr>
<td><strong>Escolaridade:</strong></td>
<td>Superior incompleto</td>
</tr>
<tr>
<td><strong>Nível de conhecimento sobre o app:</strong></td>
<td>Acabou de instalar a aplicação e não tem costume de estudar com auxílio de ferramentas de aprendizado, apesar de ter um conhecimento prévio sobre programação front-end.</td>
</tr>
<tr>
<td><strong>Intenção ao usar o aplicativo:</strong></td>
<td>Utilizar a ferramenta para estudar de modo mais dinâmico e obter resultados mais satisfatórios na Universidade.</td>
</tr>
<tr>
<td><strong>História e contexto:</strong></td>
<td> Caroline gostou da função da plataforma, do seu design e de suas funcionalidades. Também gostou da ideia de aprender colaborativamente e obter resultados em equipe, e acredita que assim participará de forma mais ativa das aulas e de maneira mais organizada em prol do seu resultado e de seu grupo, uma vez que será possível ter constantemente feedbacks dos professores e dos seus colegas de classe. Ela acredita que isso pode interferir diretamente na forma que será preparada para o mercado de trabalho.</td>
</tr>
<tr>
<td><strong>O que ele acha que poderia mudar:</strong></td>
<td>Caroline gostaria de poder visualizar também rankings individuais para fins de evolução pessoal, apesar de ter achado muito interessante os rankings somente no modo coletivo, e relatórios de desempenho no dashboard dos professores. Ela também gostaria que houvessem mais funcionalidades que integrassem os alunos, como um chat direcionado para assuntos acadêmicos, e um espaço destinado à sugestões para melhoria da ferramenta.</td>
</tr>
</tbody>
</table>

<h5 id="requisitos-elicitados-moscow">Requisitos elicitados &amp; MoSCoW</h5>
<table>
<thead>
<tr>
<th>Código</th>
<th>Descrição</th>
<th>Prioridade</th>
</tr>
</thead>
<tbody>
<tr>
<td>INS01</td>
<td>Ranking individual</td>
<td>Could have</td>
</tr>
<tr>
<td>INS02</td>
<td>Chat acadêmico.</td>
<td>Could have</td>
</tr>
<tr>
<td>INS03</td>
<td>Aba de sugestões.</td>
<td>Should have</td>
</tr>
</tbody>
</table>
<hr />

***

## 5. Referências
http://www2.dbd.puc-rio.br/pergamum/tesesabertas <br>
https://www.fm2s.com.br/metodo-moscow/
***
