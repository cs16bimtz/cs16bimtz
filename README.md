Sistema de Acompanhamento da Seleção Complementar (SASC) - Guia do utilizador 👋

### 1 - INTRODUÇÃO AO SASC
Seja bem vindo ao **Sistema de Acompanhamento da Seleção Complementar do 16º BI Mtz**. 

O Sistema de Acompanhamento da Seleção Complementar (SASC) é uma ferramenta de gestão de pessoal desenvolvida para acompanhar as diversas fases da Seleção Complementar (OM/NPOR) e proporcionar apoio à tomada de decisão. O SASC consiste de um comjunto de formulários para o cadastramento dos dados do candidato (Conscrito/Al NPOR). O formulário do SASC que realiza a coleta de dados pessoais do candidato é a Ficha Digital de Entrevista (FDE); o que coleta os dados médicos do candidato é a Ficha de Informação Médica (FIM) e o que realiza a coleta das informações odontológicas do candidato é a Ficha de Informação Odontológica (FIO). Cada formulário é composto por um conjunto de abas que agrupam campos por afinidade.

<details>
<summary>Detalhes :eye: </summary> 
 
#### 1.1 - FICHA DIGITAL DE ENTREVISTA
A FDE contempla um conjunto de grupos de dados ou abas para a coleta de informações sobre o conscrito (`DADOS PESSOAIS`, `PERFIL SOCIOECONÔMICO`, `RECRUTAMENTO POR COMPETÊNCIA`, `EXAME MÉDICO` e `EXAME ODONTOLÓGICO`), que agrupa campos de formulário respeitando a afinidade que os dados guardam entre si.

Na FDE os campos que serão utilizados como critério de seleção possuem um tipo de validação (*noempty*) que impede que os mesmos sejam armazenados com valor *NULL* no banco de dados. São campos, portanto, de preenchimento obrigatório por parte do entrevistador e foram, na medida do possível, agrupados em uma  mesma região do grupo de dados com o intuito de aumentar a legibilidade do formulário e facilitar o trabalho do entrevistador no lançamento das informações. O sistema recusará o cadastramento do conscrito se `quaisquer` dos campos abaixo, não forem corretamente preenchidos: 

 #### - DADOS PESSOAIS
 - NOME;
 - APELIDO; 
 - CPF;
 - DATA APRES CS; 
 - VOLUNTÁRIO
 
 #### - PERFIL SOCIOECONÔMICO
 - EM CASO DE CONVOCAÇÃO
 - ESTADO CIVIL; 
 - RELIGIÃO;
 - ARRIMO DE FAMÍLIA;
 - PASSAGEM PELA POLÍCIA;
 - USOU ARMA DE FOGO;
 - EXPERIÊNCIA COM DROGAS;
 - ESCOLARIDADE;
 - ENTREVISTADOR

O campo CPF do formulário tem validação *isunique*, garantindo que cada CPF armazenado no banco de dados seja único. O sistema não permitirá a duplicidade de registros. 

A FDE apresenta uma série de vantagens quando comparada à Ficha de Entrevista padrão (impressa): 
- A quase totalidade dos campos da FDE são do tipo *dropdow* (botões com alternância de visibilidade de listas, também chamados de listas suspensas), *checkbox* (caixas de checagem) ou *radiobuton* (recurso que permite ao usuário selecionar apenas um ítem entre vários). A utilização desses recursos de formulário na FDE, reduz drasticamente o tempo de entrevista por candidato em virtude da simplicidade e da rapidez no preenchimento dos dados;
- As FDE que serão impressas, assinadas e arquivadas ao final do processo (véspera de incorporação) serão as dos conscritos `CLASSIFICADOS` no processo seletivo, apenas;

#### 1.2 - GRUPOS DE DADOS
A inserção ou cadastro do conscrito no sistema só pode ser realizada por entrevistadores (abas `DADOS PESSOAIS`, `PERFIL SOCIOECONÔMICO` e `RECRUTAMENTO POR COMPETÊNCIA`). 

Médico e dentista só estão autorizados a inserir dados no cadastro dos conscritos nas abas `EXAME MÉDICO`, e `EXAME ODONTOLÓGICO` respectivamente. 

De outra forma: entrevistador realiza o cadastro do conscrito no SASC via FDE; médico e dentista preenchem os campos das abas que lhe correspondem, completando o cadastro do conscrito com informações sanitárias necessárias, cada qual em sua aba proprietária.

>**Warning**
> De forma geral, entrevistadores, médico e dentista visualizam os dados uns dos outros, mas sem permissão para edição dos campos que não sejam os do(s) seu(s) grupo(s).

Os grupos de dados (abas) da FDE são vistos por todos os usuários do sistema, todavia, existem campos em determinados grupos, que foram concebidos como campos de preenchimento exclusivo pelo presidente da CS. Tais campos não são visíveis dentro do grupo pelos demais membros da CS (entrevistadores, médico e dentista) quando logados no sistema.

Algo parecido foi aplicado aos campos das abas EXAME MÉDICO, e EXAME ODONTOLÓGICO. Tais campos, embora visíveis para todos os membros da CS, só podem ser manipulados (edição) pelo médico ou dentista da CS. Diferentemente dos campos ocultos exclusivos do presidente da CS, aqui os campos são visíveis, mas bloqueados, exceto para o médico e o dentista, cada um em sua respectiva aba "proprietária". O médico vê, mas não altera os dados na aba do dentista e vice-versa.

#### 1.3 - APRESENTAÇÃO DOS GRUPOS DE DADOS PREENCHIDOS PELO ENTREVISTADOR
<details>
<summary>FICHA DIGITAL DE ENTREVISTA (Destaque para a aba "DADOS PESSOAIS) :eye: </summary> 
 
![DP](https://user-images.githubusercontent.com/121310141/210562956-79a65c24-df13-4fba-84df-ab1bed90c068.png)

</details>
 
 
<details>
<summary>FICHA DIGITAL DE ENTREVISTA (Destaque para a aba "PERFIL SOCIOECONÔMICO") :eye: </summary> 
  
![PS](https://user-images.githubusercontent.com/121310141/210563115-6497671f-9aa1-44ef-a6bd-884ad5410b62.png)

</details>
 
 
 <details>
<summary>FICHA DIGITAL DE ENTREVISTA (Destaque para a aba "RECRUTAMENTO POR COMPETÊNCIA") :eye: </summary> 
 
![TH](https://user-images.githubusercontent.com/121310141/210563508-f7dce862-b817-4d8c-900d-bb9a33b9335b.png)

</details>

### 2 - AMBIENTE CUSTOMIZADO PARA CADA PERFIL NO SASC:
Cada usuário do sistema tem um ambiente personalizado de acordo com o seu perfil de usuário do SASC. Em cada menu estão disponíveis consultas predefinidas de acordo com o perfil do usuário. 

<details>
<summary>CMT OM 👁️ </summary> 

![CS - CMT OM](https://user-images.githubusercontent.com/121310141/210225159-d4219ef2-9ebc-428d-a149-b3e9cbf95744.png)
 
</details>
 
<details>
<summary>PRESIDENTE DA CS 👁️ </summary> 
 
![CS - PRESIDENTE](https://user-images.githubusercontent.com/121310141/210188611-259ba03b-b855-499e-b605-0ce879cc6a0a.png)

</details>

<details>
<summary>MÉDICO DA CS:eye: </summary> 
 
![CS - MEDICO](https://user-images.githubusercontent.com/121310141/210188616-530722ea-832d-48d6-a797-38d6cda4eb5b.png)

</details>

<details>
<summary>DENTISTA DA CS :eye: </summary> 
 
![CS - DENTISTA](https://user-images.githubusercontent.com/121310141/210188623-529f82a5-2408-4e9a-8172-d4cedc2d569d.png)

</details>

<details>
<summary>ENTREVISTADOR DA CS :eye: </summary> 
 
![CS - ENTREVISTADOR](https://user-images.githubusercontent.com/121310141/210188631-cbf172de-6d2e-4ff9-ad14-fb7b069f1ebc.png)

</details>
 

A tabela de permissões define quais perfis têm permissão para inserir (create), editar (update) e visualizar (read) os `campos de formulário` dentro de cada aba da FDE.
|   ID  |NOME DO UTILIZADOR               |      USUÁRIO     | SENHA | DADOS PESSOAIS |PERFIL SOCIO|  REC/COMPETÊNCIA  |EXM MED|EXM ODONTO|
|:-----:|---------------------------------|:----------------:|:-----:|:--------------:|:----------:|:-----------------:|:-----:|:--------:|
|  143  | Cmt OM!                         |          cmt_om  | root  |                |            |                   |       |          |
|  138  | Presidente da CS!               |   presidente_cs  | root  |                |            |                   |       |          |
|  139  | 2º Ten Mateus Diniz!            |        medico_1  | root  |                |            |                   |       |          |
|  146  | 2º Ten Fernandes Lopes!         |        medico_2  | root  |                |            |                   |       |          |
|  142  | 1º Ten Gadelha!                 |      dentista_1  | root  |                |            |                   |       |          |
|  137  | 2º Sgt Monteiro!                | entrevistador_1  | root  |                |            |                   |       |          |
|  140  | 2º Sgt Samuel Santos!           | entrevistador_2  | root  |                |            |                   |       |          |
|  141  | 1º Sgt Bispo!                   | entrevistador_3  | root  |                |            |                   |       |          |
|  147  | 2º Sgt Kaio!                    | entrevistador_4  | root  |                |            |                   |       |          |
|  148  | 2º Sgt Melquisedeque!           | entrevistador_5  | root  |                |            |                   |       |          |
|  149  | 3º Sgt Yago Silva!              | entrevistador_6  | root  |                |            |                   |       |          |
|  150  | 3º Sgt Ramires!                 | entrevistador_7  | root  |                |            |                   |       |          |
|  151  | 3º Sgt Fillipe!                 | entrevistador_8  | root  |                |            |                   |       |          |
|  152  | 3º Sgt Fernando Pereira!        | entrevistador_9  | root  |                |            |                   |       |          |
|  153  | Entrevistador 10!               | entrevistador_10 | root  |                |            |                   |       |          |
|  145  | Cb Romenyk!                     | aux1secao_1      | root  |                |            |                   |       |          |


- As senhas serão redefinidas por ocasião da CS e o sistema hospedado no endereço https://www.cse16bimtz.org/, será implantado no servidor da OM em https://10.46.40.34; 
- Cada entrevistador tem visibilidade apenas dos seus conscritos entrevistados;
- Os critérios para a `APROVAÇÃO` do conscrito no processo seletivo embora pareçam óbvios, não são de inteiro conhecimento do entrevistador; 
- O Ch CSC tem a visibilidade de todos os campos de preenchimento da FDE, podendo alterar e salvar informações inseridas por terceiros exceto nas abas `EXAME MÉDICO` e `EXAME ODONTO`;
- O entrevistador tem perfil com permissão para inserir e editar dados em qualquer campo de formulário da FDE, exceto nos campos das abas `EXAME MÉDICO` e `EXAME ODONTO` de preenchimento exclusivo do médico e do dentista respectivamente;
- O médico não consegue inserir nem editar campos em outra aba que não seja a sua;
- O dentista não consegue inserir nem editar campos de formulário da FDE em outra aba que não a sua.
   
### 3 - CARACTERÍSTICAS DO SASC
No SASC os atributos/características desejáveis no conscrito (Perfil do Conscrito) são os parametros que foram configurados (setados) no sistema e que podem ser alterados a critéro do Cmt OM.

O sistema terá as configurações necessárias para garantir que todos os conscritos selecionados (CLASSIFICADOS) para a incorporação, atendam aos requisitos que a unidade deseja. 

Para que o conscrito seja considerado <kbd>INDICADO</kbd> na entrevista, uma série de requisitos devem ser satisfeitos; para que o conscrito seja <kbd>CONTRAINDICADO</kbd> na fase de entrevista, todavia, basta que apenas um dos parâmetros (requisitos) não seja atendido. Essas características do sistema garantem o rigor e a homogeneidade do processo seletivo. 

Principais características do **`SASC/16º BI Mtz`**:
- É um sistema de gestão e controle;
- Permite o controle eficiente de cada uma das fases da CS;
- Controle de acesso de usuário (grupos de usuários com acesso de visualização e edição);
- Abstração do uso de papel e de impressão ao longo de praticamente toda a realização da CS;
- Ficha Digital de Entrevista (FDE); 
- Relatórios (Consultas) predefinidos no sistema: 
   - Indicados/Contraindicados na Entrevista;   
   - Aptos/Inaptos no exame médico; 
   - Aptos/Inaptos no exame odontológico;     
   - Voluntários/Não voluntários;   
   - Possuem/Não possuem habilidades;   
   - Classificados/Não classificados para a incorporação;   
   - Outras consultas (Conscritos/Estado Civil, Conscritos/Escolaridade, Conscritos/Religião, etc...)  
- Ferramenta de busca avançada; 
- Impressão da Ficha de Entrevista gerada (Apenas para os candidatos classificados);
- Imprime e exporta consultas PDF, CSV;
- Formulário para cadastramento de entrevistadores;
- Log de ações do usuário (auditoria); 
- A adoção do SASC contempla uma fase de divulgação de resultados (classificação) para os conscritos aprovados no processo de seleção complementar;
- Menu de opções: os menus agrupam, também por afinidade, as diversas consultas (relatórios) disponíveis no SASC;

<details>
<summary>LISTA DOS CONSCRITOS VOLUNTÁRIOS/ENTREVISTADOR (Exemplo de consulta) :eye: </summary> 
 
![CS - CONSCRITOS VOLUNTARIOS](https://user-images.githubusercontent.com/121310141/210190679-961a4b22-bc52-4e95-9e42-e85ecba714c2.png)

</details>

### 4 - TERMINOLOGIA/FASE DA `COMISSÃO DE SELEÇÃO` NO SASC
|  Nº FASE |DESCRIÇÃO DA FASE|      CONFORME  |   NÃO CONFORME  |  OBS | 
|:--------:|-----------------|:--------------:|:---------------:|:----:|
|  1       | ENTREVISTA      |  INDICADO      | CONTRAINDICADO  |  -   | 
|  2       | EXAME MÉDICO    |  APTO          | INAPTO          |  -   |
|  3       | EXAME ODONTO    |  APTO          | INAPTO          |  -   | 
|  4       | TESTE HABILIDADE|  DEMONSTROU    | NÃO DEMONSTROU  |  -   | 
|  5       | RESULTADO FINAL CS |  APROVADO      | REPROVADO       |    |
|  5       | PARA A INCORPORAÇÃO    |  CLASSIFICADO  | NÃO CLASSIFICADO|  -   | 

- Na fase de entrevista o sistema adota os termos **INDICADO** e **CONTRAINDICADO** para significar que o conscrito `atende/não atende` aos requisitos exigidos; 

- Ao longo do exame médico e do exame odontológico os termos utilizados são **APTO** e **INAPTO** para indicar que o conscrito `possui/não possui` as características físicas e a higidez que se deseja em um soldado; 

- Na fase aonde são verificadas as habilidades declaradas pelo conscrito na FDE, os termos utilizados são **demonstrou** e **não demonstrou** a competência declarada;

- Na etapa aonde são processados (analisados) os dados coletados, os termos utilizados são **CLASSIFICADO** e **NÃO CLASSIFICADO** para indicar que o conscrito foi `selecionado/não selecionado` para a incorporação. 

> **Note**
> <kbd>INDICADO</kbd> &ne; <kbd>APTO</kbd> &ne; <kbd>AROVADO</kbd> &ne; <kbd>CLASSIFICADO</kbd>

### 5 - PARÂMETROS DE CONFIGURAÇÃO UTILIZADOS NO SASC:
#### Parametrização de alguns dos campos de formulário da aba `DADOS PESSOAIS`, para o conscrito ser considerado <kbd>INDICADO</kbd> na fase 1 (ENTREVISTA) do processo seletivo:
 ABA DE DADOS DO FORMULÁRIO |            CAMPO DE FORMULÁRIO      |     CONDIÇÃO (CRITÉRIO OU PARÂMETRO UTILIZADO)     | STATUS   | OBS                          |
----------------------------|-------------------------------------|----------------------------------------------------|----------|------------------------------|
 DADOS PESSOAIS             | ESTADO CIVIL                        | = Solteiro                                           | INDICADO |                              |
 DADOS PESSOAIS             | RELIGIÃO                            | &ne; Adventista                                       | INDICADO |Não pode ser adventista       |
 DADOS PESSOAIS             | ESCOLARIDADE                        | &ne; Ensino fundamental incompleto                    | INDICADO |Pelo menos o EF completo      |
 DADOS PESSOAIS             | VOLUNTÁRIO                          | = Sim                                                | INDICADO |                              |
 DADOS PESSOAIS             | OUTROS CAMPOS                       | OUTROS CRITÉRIOS                                             | INDICADO |                              |

- No campo `RELIGIÃO` da aba DADOS PESSOAIS, se o valor selecionado for "Adventista", o conscrito será automaticamente contraindicado, independente de quais sejam as respostas para os demais campos utilizados como parâmetros na aba considerada. Lembre-se de que esse é um campo com validação (*noempty*). O entrevistador é impedido de salvar/cadastrar as demais informações do conscrito se esse campo não for preenchido.  

- Não existe no sistema o botão `Indicado`, ou `Indicar candidato`, ou `Indicar conscrito`. Essa tarefa foi automatizada, significando dizer que o próprio sistema se encarregará de indicar (ou contraindicar) o conscrito a partir dos dados coletados na FDE em confronto com os parâmetros configurados.
 
 - A situação de contraindicado durante a fase de entrevista, depende da negação de apenas um dos parâmetros das abas DADOS PESSOAIS  e PERFIL SOCIOECONÔMICO.

#### Parametrização de alguns dos campos de formulário da aba `PERFIL SOCIOECONÔMICO` para o conscrito ser considerado <kbd>Indicado</kbd> ainda na fase 1 (ENTREVISTA) do processo seletivo:
 ABA DE DADOS DO FORMULÁRIO |            CAMPO DE FORMULÁRIO      |     CONDIÇÃO (CRITÉRIO OU PARÂMETRO UTILIZADO)     | STATUS   | OBS                          |
----------------------------|-------------------------------------|----------------------------------------------------|----------|------------------------------|
 PERFIL SOCIOECONÔMICO      | `MORA COM QUEM NO ENDEREÇO DECLARADO` | = Pais                                               | INDICADO |                              |
 PERFIL SOCIOECONÔMICO      | EM CASO DE CONVOCAÇÃO               | &ne; Adotarei o aquartelamento como residência     | INDICADO |Não pode querer ser laranjeira|
 PERFIL SOCIOECONÔMICO      | ARRIMO DE FAMÍLIA                   | = Não                                                | INDICADO |                              |
 PERFIL SOCIOECONÔMICO      | PASSAGEM PELA POLÍCIA               | = Não                                                | INDICADO |                              |
 PERFIL SOCIOECONÔMICO      | EXPERIÊNCIA COM DROGAS              | = Não                                                | INDICADO |                              |
 PERFIL SOCIOECONÔMICO      | USO DE ARMA DE FOGO                 | = Não                                                | INDICADO |                              |

- No campo denominado `MORA COM QUEM NO ENDEREÇO DECLARADO` da aba PERFIL SOCIOECONÔMICO, se o valor selecionado for diferente de "Pais", o conscrito será automaticamente <kbd>CONTRAINDICADO</kbd>, independente de quais sejam as respostas para os demais campos utilizados como parâmetros na aba considerada. Repare que os critérios podem ser tão rigorosos quanto possível. Nesse batalhão hipotético todos os conscritos devem morar com os pais, porque morar com os pais pressupõe que o candidato seja detentor de valores morais e éticos que só podem ser adquiridos a partir da convivência em família, valores esses, essenciais à vida na caserna.

#### Parametrização de alguns dos campos de formulário da aba `EXAME MÉDICO` para o conscrito ser considerado <kbd>Apto</kbd> na fase 2 (EXAME MÉDICO) do processo seletivo:
 ABA DE DADOS DO FORMULÁRIO |            CAMPO DE FORMULÁRIO      |     CONDIÇÃO (CRITÉRIO OU PARÂMETRO UTILIZADO)     | STATUS   | OBS                          |
----------------------------|-------------------------------------|----------------------------------------------------|----------|------------------------------|
 EXAME MÉDICO               | PARECER MÉD            | = Apto                                                | APTO     |                              |
 

#### Parametrização de alguns dos campos de formulário da aba `EXAME ODONTOLÓGICO` para o conscrito ser considerado <kbd>Apto</kbd> na fase 3 (EXAME ODONTO) do processo seletivo:
 ABA DE DADOS DO FORMULÁRIO |            CAMPO DE FORMULÁRIO      |     CONDIÇÃO (CRITÉRIO OU PARÂMETRO UTILIZADO)     | STATUS   | OBS                          |
----------------------------|-------------------------------------|----------------------------------------------------|----------|------------------------------|
 EXAME ODONTO               | QNT DE CÁRIE DE ESMALTE (CE)             | <=3  (por exemplo)                                 | APTO     |                              |
 EXAME ODONTO               | QNT DE CÁRIE DE DENTINA (CD)             | <=3  (por exemplo)                                 | APTO     |                              |
 EXAME ODONTO               | QNT RESTAURAÇÕES INADEQUADAS(RI)        | <=3  (por exemplo)                                 | APTO     |                              |
 EXAME ODONTO               | QNT AUSÊNCIA DENT ANTERIOR (ADA)        | <=3  (por exemplo)                                 | APTO     |                              |
 EXAME ODONTO               | QNT AUSÊNCIA DENT POSTERIOR (ADP)        | <=3  (por exemplo)                                 | APTO     |                              |

### 6 - STATUS DO CONSCRITO AO FINAL DA SELEÇÃO/CASOS (1-5)
|   CASO  | ENTREVISTA  | EXAME MÉDICO |EXAME ODONTO|TESTE DE HABILIDADES| RESULTADO CS | CLASSIFICAÇÃO|
| :-----: | :---------: | :----------: | :----------: | :------------------: |:-------:|-----|
| 1       |🔵    |🔵      |🔵     |🔵  |   APROVADO|⭐⭐⭐⭐⭐|
| 2       |🔵    |🔵      |🔵     |🔴  |   APROVADO|⭐⭐⭐⭐|
| 3       |🔵    |🔵      |🔴     |     |  REPROVADO |  -  |
| 4       |🔵    |🔴      |       |     | REPROVADO    |  -  |
| 5       |🔴    |        |       |     |   REPROVADO   |  - | 

- Conscrito contraindicado na entrevista não realiza a fase seguinte conforme Caso 5 da tabela STATUS/CASO.

- Conscrito `Não conforme` em uma das fases não realiza a triagem na fase seguinte (Casos 3, 4 e 5). 

### 7 - MÉTODO PARA A CLASSIFICAÇÃO DOS CONSCRITOS (⭐⭐⭐⭐)
#### 7.1 - FERRAMENTA DE BUSCA AVANÇADA DO SASC
A classificação dos conscritos poderá ser feita solicitando à **base de dados** de conscritos uma consulta que atenda a um conjunto de critérios. 

Exemplo de consulta à base de dados do sistema utilizando a ferramenta de busca avançada: desejamos que o sistema nos retorne uma consulta (lista) dos conscritos que sejam solteiros ou divorciados, morem com os pais, possuam o ensino médio completo, sejam católicos ou espíritas ou evangélicos, tenham tipo sanguíneo O+ ou A+, CNH Cat D ou E, que não sejam usuários de droga, não tenham passagem pela polícia, não sejam arrimo de família, que possuam qualquer conhecimento de TIC, sejam  praticantes de natação ou basquete, e que residam no Tirol ou em Capim Macio ou em Petrópolis, cujo nome do pai tenha "R" como primeira letra, não sejam portadores de transtornos ansiosos ou depressivos, não estejam ou tenham passado por tratamento psicológico ou psiquiátrico, sejam voluntários e que tenham menos que cinco cáries, etc.

A consulta retornada poderia ser a relação dos conscritos classificados no processo, por exemplo. 

> **Warning**
> O único cuidado que se deve ter é fazer constar na pesquisa, exatamente todos os parâmetros que foram utilizados ao longo das diversas fases da CS para indicar/contraindicar (ENTREVISTA), ou capacitar/incapacitar (EXAME MÉDICO e EXAME ODONTOLÓGICO) o conscrito. A pesquisa acima traria os conscritos portadores de epilepsia como conscritos classificados, e os que possuem habilidades na área da construção civil (pedreiro, pintor, encanador, etc) como não classificados, o que seria uma falha grave.

#### 7.2 - UTILIZANDO CONSULTA PREDEFINIDA NOS MENUS DO SASC
O sistema dispõe das seguintes consultas predefinidas:

- CONSCRITOS APRESENTADOS
- CONSCRITOS VOLUNTÁRIOS
- CONSCRITOS APROVADOS
- CONSCRITOS CLASSIFICADOS
- CONSCRITOS INDICADOS (FASE - 1)
- CONSCRITOS APTOS NO EXAME MÉDICO (FASE - 2)
- CONSCRITOS APTOS NO EXAME ODONTOLÓGICO (FASE - 3)
- CONSCRITOS QUE DEMONSTRARAM ALGUMA HABILIDADE (FASE -4)
- OUTRAS

Estabelecendo para a `CLASSIFICAÇÃO` o critério de avaliação maior ou igual a ⭐⭐⭐, não seriam classificados:
- Encanador: ⭐⭐ (Aprovado, não classificado);
- Eletricista: ⭐ (Aprovado, não classificado), etc.
 
|  Nº |DESCRIÇÃO DA HABILIDADE|RESULTADO CS |  AVALIAÇÃO   |  CLASSIFICAÇÃO    |
|:---:|-----------------------|:--------:|:------------|:---------------:|
|  1       | Pedreiro         | APROVADO |⭐⭐⭐⭐⭐ | CLASSIFICADO  |
|  2       | Carpinteiro      | APROVADO |⭐⭐⭐⭐   | CLASSIFICADO   |
|  3       | Pintor           | APROVADO |⭐⭐⭐      | CLASSIFICADO    |
|  4       | Encanador        | APROVADO |⭐⭐         | NÃO CLASSIFICADO|
|  5       |Eletricista       | APROVADO |⭐           | NÃO CLASSIFICADO|

Existe uma consulta definida no sistema para exibir os classificados que atendam a esses critérios.
 
### 8 -  MÉTODO PARA A DISTRIBUIÇÃO POR SUBUNIDADE
Feita pelo Presidente da CS. Pode ser realizada manualmente, ou automatizada a patir de critérios.

Exemplo: Cria-se a consulta 2ª Cia Fuz, que agrupará todos os conscritos classificados com três ou mais ⭐⭐⭐, cujo valor armazenado no campo ALTURA (cm) seja maior que 170 (cm), por exemplo.
 
### 9 - FASEAMENTO DE UMA CS PARA O MELHOR DESEMPENHO DO SASC
 
 <details>
<summary>DIAGRAMA DE FASES DA CS :eye: </summary> 

![CS Diagrama (7)](https://user-images.githubusercontent.com/121310141/210290692-5cf51a34-5aa7-4755-8bd8-1710691e9afd.png)
  
</details>


 ### 10 - QUADRO DE DISTRIBUIÇÃO DOS CONSCRITOS POR GRUPAMENTO
|Nº  |   DATA     |EVENTO        |        A      |      B     |      C      |      D       |      E    |   
|:--:|:----------:|:------------:|:-------------:|:----------:|:-----------:|:------------:|:---------:|
| 1  | 16/01/2023 | APRESENTAÇÃO |        -      |      -     |     -       |        -     |    -      | 
| 2  | 17/01/2023 |       -      |    TRIAGEM    |      -     |     -       |        -     |    -      | 
| 3  | 18/01/2023 |       -      |        -      |  TRIAGEM   |     -       |        -     |    -      | 
| 4  | 19/01/2023 |       -      |        -      |      -     |   TRIAGEM   |        -     |    -      |
| 5  | 20/01/2023 |       -      |        -      |      -     |     -       |    TRIAGEM   |    -      |
| 6  | 23/01/2023 |       -      |        -      |      -     |     -       |        -     | TRIAGEM   | 
| 7  | 24/01/2023 |       -      |   TESTE HBL   |      -     |     -       |        -     |    -      |
| 9  | 25/01/2023 |       -      |               |  TESTE HBL |     -       |        -     |    -      |
| 10 | 26/01/2023 |       -      |        -      |      -     |   TESTE HBL |        -     |    -      |
| 11 | 27/01/2023 |       -      |        -      |      -     |      -      |   TESTE HBL  |    -      |
| 12 | 30/01/2023 |       -      |        -      |      -     |     -       |        -     | TESTE HBL | 
| 13 | 31/01/2023 |  RESULTADO   |        -      |      -     |     -       |        -     |     -     | 

 
 
<hr>
 
### 11 - DICAS 
 
 1 - FAZ A PERGUNTA, OLHA O CONSCRITO NOS OLHOS, ESPERA ELE FALAR SEM INTERROMPÊ-LO, DEPOIS FAZ O LANÇAMENTO;
 
 2 - O CONSCRITO DEVE PERCEBER QUE O ENTREVISTADOR ESTÁ ATENTO AO QUE ELE ESTÁ FALANDO;

 3 - ENTREVISTADOR DEVE EVITAR SE DISTRAIR COM O CELULAR DURANTE A ENTREVISTA;
 
 4 - ALGUMAS TÉCNICAS: USE O APELIDO AO SE DIRIGIR AO CONSCRITO, ELE VAI SE SENTIR CONFORTÁVEL;
 
 5 - MÁXIMO DE RESPEITO COM O CONSCRITO;
 
 6 - ENTREVISTADOR NÃO DEVE FAZER COMENTÁRIOS DE QUALQUER NATUREZA SOBRE AS RESPOSTAS/OPINIÕES DO CONSCRITO;
 
 7 - TENTAR FAZER A ENTREVISTA FLUIR.
</details>


 
 
