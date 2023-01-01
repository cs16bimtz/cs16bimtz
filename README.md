Sistema de Acompanhamento da Seleção Complementar (SASC) - Guia do utilizador 👋

### 1 - INTRODUÇÃO AO SASC
Seja bem vindo ao **Sistema de Acompanhamento da Seleção Complementar do 16º BI Mtz**. 

O SASC é um sistema de gestão e foi concebido para ser a ferramenta de levantamento e análise de dados dos conscritos durante e após a execução da seleção complementar na OM. 

É composto basicamente de um formulário de cadastro denominado **Ficha Digital de Entrevista (FDE)** cujos campos são os campos da Ficha de Entrevista do Conscrito nos moldes como a conhecemos (a que se encontra anexa à Ordem de Serviço para execução da CS). 

#### 1.1 - FICHA DIGITAL DE ENTREVISTA
A FDE contempla um conjunto de grupos de dados ou abas para a coleta de informações sobre o conscrito (`DADOS PESSOAIS`, `TÍTULO DE ELEITOR`, `CNH`, `EXAME MÉDICO`, `EXAME ODONTOLÓGICO`, `TESTE DE HABILIDADES`, `PERFIL SOCIOECONÔMICO`, etc), que agrupa campos de formulário respeitando a afinidade que os dados guardam entre si.

Na FDE os campos que serão utilizados como critério de seleção possuem um tipo de validação (*noempty*) que impede que os mesmos sejam armazenados com valor *NULL* no banco de dados. São campos, portanto, de preenchimento obrigatório por parte do entrevistador e foram, na medida do possível, agrupados em uma  mesma região do grupo de dados com o intuito de aumentar a legibilidade do formulário e facilitar o trabalho do entrevistador no lançamento das informações.

A FDE apresenta uma série de vantagens quando comparada à Ficha de Entrevista padrão (impressa): 
- A quase totalidade dos campos da FDE são do tipo *dropdow* (botões com alternância de visibilidade de listas, também chamados de listas suspensas), *checkbox* (caixas de checagem) ou *radiobuton* (recurso que permite ao usuário selecionar apenas um ítem entre vários). A utilização desses recursos de formulário na FDE, reduz drasticamente o tempo de entrevista por candidato em virtude da simplicidade e da rapidez no preenchimento dos dados;
- As FDE que serão impressas, assinadas e arquivadas ao final do processo (véspera de incorporação) serão as dos conscritos `CLASSIFICADOS` no processo seletivo, apenas;

#### 1.2 - GRUPOS DE DADOS
A inserção ou cadastro do conscrito no sistema só pode ser realizada por entrevistadores (abas `DADOS PESSOAIS`, `TÍTULO DE ELEITOR`, `CNH`, `PERFIL SOCIOECONÔMICO`). 

Médico e dentista só estão autorizados a inserir dados no cadastro dos conscritos nas abas `EXAME MÉDICO`, e `EXAME ODONTOLÓGICO` respectivamente. De outra forma: entrevistador realiza o cadastro do conscrito no SASC via FDE, médico e dentista preenchem os campos das abas que lhe correspondem, completando o cadastro do conscrito com informações sanitárias necessárias, cada qual em sua aba proprietária.

>**Warning**
> De forma geral, entrevistadores, médico e dentista visualizam os dados uns dos outros, mas sem permissão para edição dos campos que não sejam os do(s) seu(s) grupo(s).não podem inserir um conscrito no sistema, mas podem visualizar os dados dos conscritos inseridos pelos entrevistadores sem no entanto, poder editar tais dados. 

Os grupos de dados (abas) da FDE são vistos por todos os usuários do sistema, todavia, existem campos em determinados grupos, que foram concebidos como campos de preenchimento exclusivo pelo presidente da CS. Tais campos não são visíveis dentro do grupo pelos demais membros da CS (entrevistadores, médico e dentista) quando logados no sistema.

Algo parecido foi aplicado aos campos das abas EXAME MÉDICO, e EXAME ODONTOLÓGICO. Tais campos, embora visíveis para todos os membros da CS, só podem ser manipulados (edição) pelo médico ou dentista da CS. Diferentemente dos campos ocultos exclusivos do presidente da CS, aqui os campos são visíveis, mas bloqueados, exceto para o médico e o dentista, cada um em sua respectiva aba "proprietária". O médico vê, mas não altera os dados na aba do dentista e vice-versa.

De forma geral, entrevistadores, médico e dentista visualizam os dados uns dos outros, mas sem permissão para edição dos campos que não sejam os do(s) seu(s) grupo(s).

### 2 - APRESENTAÇÃO DOS GRUPOS DE DADOS:
<details>
<summary>DADOS PESSOAIS</summary> 
 
![dados_pessoais](https://user-images.githubusercontent.com/121310141/210165676-6ef36d84-1c92-4bcc-9627-b69f00407a9e.png)

Na imagem acima temos a aba DADOS PESSOAIS da Ficha "Digital" de Entrevista do Conscrito em evidência. 

Repare que o sistema recusa o cadastramanto do conscrito se `quaisquer` dos campos: NOME, CPF, ESTADO CIVIL, RELIGIÃO, ESCOLARIDADE, VOLUNTÁRIO ou ENTREVISTADOR não forem corretamente preenchidos.  

O campo CPF do formulário tem validação *isunique*, garantindo que cada CPF armazenado no banco de dados seja único. De outra forma: o sistema não permitirá a duplicidade de cadastro.  
</details>

<details>
<summary>TÍTULO DE ELEITOR</summary> 
 
![dados_pessoais](https://user-images.githubusercontent.com/121310141/210165676-6ef36d84-1c92-4bcc-9627-b69f00407a9e.png)
  
</details>

<details>
<summary>CNH</kbd></summary>
 
![fm](https://user-images.githubusercontent.com/121310141/209503889-b8d7322c-934d-472d-895f-1b6718a2b76d.png)

Na imagem acima temos a aba DADOS PESSOAIS da Ficha "Digital" de Entrevista do Conscrito em evidência. 
 > **Note**
> Repare que o sistema recusa o cadastramanto do conscrito se `quaisquer` dos campos: NOME, CPF, ESTADO CIVIL, RELIGIÃO, ESCOLARIDADE, VOLUNTÁRIO ou ENTREVISTADOR não forem corretamente preenchidos. 

> **Note**
> O campo CPF do formulário tem validação *isunique*, garantindo que cada CPF armazenado no banco de dados seja único. De outra forma: o sistema não permitirá a duplicidade de cadastro.  
</details>
  
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
- A adoção do SASC contempla uma fase de divulgação de resultados (classificação) para os conscritos aprovados no processo de seleção complementar.
- Menu de opções: os menus agrupam, também por afinidade, as diversas consultas (relatórios) disponíveis no SASC.

### 4 - TERMINOLOGIA/FASE DA `COMISSÃO DE SELEÇÃO` NO SisASC
|  Nº FASE |DESCRIÇÃO DA FASE|      CONFORME  |   NÃO CONFORME  |  OBS | 
|:--------:|-----------------|:--------------:|:---------------:|:----:|
|  1       | ENTREVISTA      |  INDICADO      | CONTRAINDICADO  |  -   | 
|  2       | EXAME MÉDICO    |  APTO          | INAPTO          |  -   |
|  3       | EXAME ODONTO    |  APTO          | INAPTO          |  -   | 
|  4       | TESTE HABILIDADE|  DEMONSTROU    | NÃO DEMONSTROU  |  -   | 
|  5       | RESULTADO FINAL CS |  APROVADO      | REPROVADO       |    |
|  5       | PARA A INCORPORAÇÃO    |  CLASSIFICADO  | NÃO CLASSIFICADO|  -   | 

- Na fase de entrevista o sistema adota os termos **indicado** e **contraindicado** para significar que o conscrito `atende/não atende` aos requisitos exigidos; 

- Ao longo do exame médico e do exame odontológico os termos utilizados são **apto** e **inapto** para indicar que o conscrito `possui/não possui` as características físicas e a higidez que se deseja em um soldado; 

- Na fase aonde são verificadas as habilidades declaradas pelo conscrito na FDE, os termos utilizados são **demonstrou** e **não demonstrou** a competência declarada;

- Finalizada a CS, os candidatos estarão distribuídos em dois grupos (APROVADOS/REPROVADOS). Os aprovados serão em número a maior em relação à quantidade de vagas disponíveis e os reprovados, esses foram dispensados ao longo das diversas fases da CS;

- Na etapa onde são processados os dados coletados os termos utilizados são **classificado** e **não classificado** para indicar que o conscrito foi `selecionado/não selecionado` para a incorporação. 

> **Note**
> <kbd>INDICADO</kbd> &ne; <kbd>APTO</kbd> &ne; <kbd>AROVADO</kbd> &ne; <kbd>CLASSIFICADO</kbd>


### 5 - PARÂMETROS DE CONFIGURAÇÃO UTILIZADOS NO SisASC:
#### Parametrização de alguns dos campos de formulário da aba `DADOS PESSOAIS`, para o conscrito ser considerado <kbd>INDICADO</kbd> na fase 1 (ENTREVISTA) do processo seletivo:
 ABA DE DADOS DO FORMULÁRIO |            CAMPO DE FORMULÁRIO      |     CONDIÇÃO (CRITÉRIO OU PARÂMETRO UTILIZADO)     | STATUS   | OBS                          |
----------------------------|-------------------------------------|----------------------------------------------------|----------|------------------------------|
 DADOS PESSOAIS             | ESTADO CIVIL                        | = Solteiro                                           | INDICADO |                              |
 DADOS PESSOAIS             | RELIGIÃO                            | &ne; Adventista                                       | INDICADO |Não pode ser adventista       |
 DADOS PESSOAIS             | ESCOLARIDADE                        | &ne; Ensino fundamental incompleto                    | INDICADO |Pelo menos o EF completo      |
 DADOS PESSOAIS             | VOLUNTÁRIO                          | = Sim                                                | INDICADO |                              |

- No campo `RELIGIÃO` da aba DADOS PESSOAIS, se o valor selecionado for "Adventista", o conscrito será automaticamente contraindicado, independente de quais sejam as respostas para os demais campos utilizados como parâmetros na aba considerada. Lembre-se de que esse é um campo com validação (*noempty*). O entrevistador é impedido de salvar/cadastrar as demais informações do conscrito se esse campo não for preenchido.  

- Não existe no sistema o botão `Indicado`, ou `Indicar candidato`, ou `Indicar conscrito`. Essa tarefa foi automatizada, significando dizer que o próprio sistema se encarregará de indicar (ou contraindicar) o conscrito a partir dos dados coletados na FDE em confronto com os parâmetros configurados.

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
 EXAME MÉDICO               | TOMA REMÉDIO CONTROLADO             | = Não                                                | APTO     |                              |
 EXAME MÉDICO               | FEZ OU FAZ                          | &ne; Tratamento Psicológico                        | APTO     |                              |
 EXAME MÉDICO               | FEZ OU FAZ                          | &ne; Tratamento Psiquiátrico                       | APTO     |                              |

#### Parametrização de alguns dos campos de formulário da aba `EXAME ODONTOLÓGICO` para o conscrito ser considerado <kbd>Apto</kbd> na fase 3 (EXAME ODONTO) do processo seletivo:
 ABA DE DADOS DO FORMULÁRIO |            CAMPO DE FORMULÁRIO      |     CONDIÇÃO (CRITÉRIO OU PARÂMETRO UTILIZADO)     | STATUS   | OBS                          |
----------------------------|-------------------------------------|----------------------------------------------------|----------|------------------------------|
 EXAME ODONTO               | QNT DE CÁRIE DE ESMALTE             | <=3  (por exemplo)                                 | APTO     |                              |
 EXAME ODONTO               | QNT DE CÁRIE DE DENTINA             | <=3  (por exemplo)                                 | APTO     |                              |
 EXAME ODONTO               | QNT RESTAURAÇÕES INADEQUADAS        | <=3  (por exemplo)                                 | APTO     |                              |
 EXAME ODONTO               | QNT AUSÊNCIA DENT ANTERIOR          | <=3  (por exemplo)                                 | APTO     |                              |
 EXAME ODONTO               | QNT AUSÊNCIA DENT POSTERIOR         | <=3  (por exemplo)                                 | APTO     |                              |

- Não existe também no sistema, na fase de realização dos exames médicos/adontológicos, o botão `Apto`, ou `Conscrito apto`, ou `Conscrito inapto`. Essa tarefa também foi automatizada, significando dizer que o próprio sistema se encarregará de definir se o conscrito foi apto (ou inapto), a partir dos dados coletados na FDE em confronto com os parâmetros configurados, que por enquanto são os constantes das tabelas acima.

- A situação de contraindicado durante a fase de entrevista, depende da negação de apenas um dos parâmetros das abas DADOS PESSOAIS  e PERFIL SOCIOECONÔMICO.

### 6 - STATUS DO CONSCRITO AO FINAL DA SELEÇÃO/CASOS (1-5)
|   CASO  | ENTREVISTA  | EXAME MÉDICO |EXAME ODONTO|TESTE DE HABILIDADES| RESULTADO CS | CLASSIFICAÇÃO|
| :-----: | :---------: | :----------: | :----------: | :------------------: |:-------:|-----|
| 1       |🟢    |🟢      |🟢     |🟢  |   APROVADO|⭐⭐⭐⭐⭐|
| 2       |🟢    |🟢      |🟢     |🔴  |   APROVADO|⭐⭐⭐⭐|
| 3       |🟢    |🟢      |🔴     |     |  REPROVADO |  -  |
| 4       |🟢    |🔴      |       |     | REPROVADO    |  -  |
| 5       |🔴    |        |       |     |   REPROVADO   |  - | 

- Conscrito contraindicado na entrevista não realiza a fase seguinte conforme Caso 5 da tabela STATUS/CASO.

- Conscrito `Não conforme` em uma das fases não realiza a triagem na fase seguinte (Casos 3, 4 e 5). 

### 7 - TABELA DE USUÁRIOS DO SISTEMA E PERMISSÕES POR ABA DA FDE
A tababela de permissões trata de quais perfis dentro de cada aba tem permissão para inserir (I), editar (E), visualizar (V) os campos de formulário.
|Nº |NOME DO UTILIZADOR|      USUÁRIO   | SENHA | DADOS PESSOAIS |TIT ELEITOR|CNH|EXM MÉDICO|EXM ODONTO|HABILIDADES|PERFIL|
|:--:|-----------------|:--------------:|:---: |:--------------:|:------------:|:-:|:----------:|:----------:|:---:|:-------:|
| 1 | Cmt OM           |         cmt_om | root| ✔️           | ✔️          |✔️| ✖️        | ✖️        | ✔️      | ✔️      |
| 2 | Presidente da CS |  presidente_cs | root| ✔️           | ✔️          |✔️| ✖️        | ✖️        | ✔️      | ✔️      |
| 3 | Médico 1         |       medico_1 | root| ✖️           | ✖️          |✖️| ✔️        | ✖️        | ✖️      | ✖️      | 
| 4 | Médico 2         |       medico_2 | root| ✖️           | ✖️          |✖️| ✔️        | ✖️        | ✖️      | ✖️      | 
| 5 | Dentista         |     dentista_1 | root| ✖️           | ✖️          |✖️| ✖️        | ✔️        | ✖️      | ✖️      | 
| 6 | Entrevistador 1  |entrevistador_1 | root| ✔️           | ✔️          |✔️| ✖️        | ✖️        | ✔️      | ✔️      | 
| 7 | Entrevistador 2  |entrevistador_2 | root| ✔️           | ✔️          |✔️| ✖️        | ✖️        | ✔️      | ✔️      | 
| 8 | Entrevistador 3  |entrevistador_3 | root| ✔️           | ✔️          |✔️| ✖️        | ✖️        | ✔️      | ✔️      | 


- As senhas serão redefinidas por ocasião da CS e o sistema hospedado no servidor da OM no endereço https://10.46.40.34; 

- Cada entrevistador tem visibilidade apenas dos seus entrevistados

- Os critérios para a classificação do conscrito no processo seletivo embora pareçam óbvios, não são de inteiro conhecimento do entrevistador. 

- O Ch CSC tem a visibilidade de todos os campos de preenchimento da FDE, podendo alterar e salvar informações inseridas por terceiros;

- O entrevistador tem perfil com permissão para inserir e editar dados em qualquer campo de formulário da FDE, exceto nos campos das abas `EXAME MÉDICO` e `EXAME ODONTO` de preenchimento exclusivo do médico e do dentista respectivamente;

- O médico não consegue inserir nem editar campos em outra aba que não seja a sua;

- O dentista não consegue inserir nem editar campos de formulário da FDE em outra aba que não a sua.

- Exemplo de uso do campo de formulário PRIORIZAÇÃO da aba DADOS PESSOAIS ao final da CS e durante a análise dos dados coletados. Esse campo foi parametrizado classificando e exibindo uma consulta já definida dos conscritos aprovados cuja avaliação tenha sido >=3 estrelas:
- Pedreiro: ⭐⭐⭐⭐⭐;
- Mot Cat D: ⭐⭐⭐⭐;
- Carpinteiro: ⭐⭐⭐;
- Mecânico: ⭐⭐ (Aprovado, não classificado);
- Padeiro: ⭐ (Aprovado, não classificado), etc.









### 8 - TABELA DE PERMISSÕES
A tababela de permissões trata de quais perfis dentro de cada aba tem permissão para inserir (I), editar (), visualizar (V) os campos de formulário (exceto os campos de preenchimento exclusivo).
|  Nº |      PERFIL       | DADOS PESSOAIS |TITULO ELEITOR|CNH|EXAME MÉDICO|EXAME ODONTO|TESTE HABILIDADES|PERFIL SOCIOECONOMICO|  OBS |
|:---:|-------------------|:--------------:|:------------:|:-:|:----------:|:----------:|:---------------:|:-------------------:|:----:|
|  1  | Cmt OM            | 🟢           | 🟢          |🟢| 🔴        | 🔴        | 🟢             | 🟢                 | -    |
|  2  | Presidente da CS  | 🟢            | 🟢          |🟢| 🔴        | 🔴        | 🟢             | 🟢                 | -    |
|  3  | Médico            | 🔴              | 🔴            | 🔴 | 🟢        | 🔴          | 🔴               | 🔴                   | -    |
|  4  | Dentista          | 🔴              | 🔴            | 🔴 | 🔴          | 🟢        | 🔴               | 🔴                   | -    |
|  5  | Entrevistador     | 🟢            | 🟢          |🟢| 🔴          | 🔴          | 🟢             | 🟢                 | -    |

Legenda: 

🟢 - Visualiza, insere e altera dados nas abas proprietárias;
🔴 - Visualiza, não insere nem altera dados

- O Ch CSC tem a visibilidade de todos os campos de preenchimento da FDE, podendo alterar e salvar informações inseridas por terceiros;

- O entrevistador tem perfil com permissão para inserir e editar dados em qualquer campo de formulário da FDE, exceto nos campos das abas `EXAME MÉDICO` e `EXAME ODONTO` de preenchimento exclusivo do médico e do dentista respectivamente;

- O médico não consegue inserir nem editar campos em outra aba que não seja a sua;

- O dentista não consegue inserir nem editar campos de formulário da FDE em outra aba que não a sua.

- Exemplo de uso do campo de formulário PRIORIZAÇÃO da aba DADOS PESSOAIS ao final da CS e durante a análise dos dados coletados. Esse campo foi parametrizado classificando e exibindo uma consulta já definida dos conscritos aprovados cuja avaliação tenha sido >=3 estrelas:
- Pedreiro: ⭐⭐⭐⭐⭐;
- Mot Cat D: ⭐⭐⭐⭐;
- Carpinteiro: ⭐⭐⭐;
- Mecânico: ⭐⭐ (Aprovado, não classificado);
- Padeiro: ⭐ (Aprovado, não classificado), etc.

- Durante a análise dos dados coletados (fase pós CS) e antes da divulgação do resultado do processo seletivo, utilizando a ferramenta de busca avançada já disponível no sistema, será possível a realização de consultas como: 

Exemplo de consulta à base de dados do sistema utilizando a ferramenta de busca avançada: desejamos que o sistema nos retorne uma consulta (lista) dos conscritos aprovados na CS, que sejam solteiros ou divorciados, morem com os pais, possuam o ensino médio completo, sejam católicos ou espíritas ou evangélicos, tenham tipo sanguíneo O+ ou A+, CNH Cat D ou E, que não sejam usuários de droga, não tenham passagem pela polícia, não sejam arrimo de família, que possuam qualquer conhecimento de TIC,sejam  praticantes de natação ou basquete, e que residam no Tirol ou em Capim Maciou ou em Petrópolis, cujo nome do pai tenha "R" como primmeira letra, não sejam portadores de transtornos ansiosos ou depressivos, tenham menos que cinco cáries, etc.

 - Estado da aba: visível, oculta, visível mas bloqueada para usuários sem perfil para inserir ou editar dados nos campos da aba; 
   - Estado do campo: visível, oculto, visível 



No entanto, se durante a fase de processamento dos dados (fase pós CS), o número necessário de conscritos para o preenchimento dos `claros` não tenha sido atingido, em virtude do rigor dos parâmetros definidos no sistema, a critério do Cmt OM, tais parâmetros podem ser flexibilizados obedecendo a uma precedência definida também pelo Cmt OM, sem prejuízo para o processo. Conclui-se daí que existe uma fase aonde são coletados os dados dos conscritos (dados pessoais, dados socioeconomicos, dados médicos, etc) e uma outra fase muita curta aonde os dados coletados são processados (analisados). 

Exemplo: o Cmt da OM/Presidente da CS pode estabelecer inicialmente que todos os conscritos selecionados para a incorporação necessariamente devam residir no município de Natal (campo ENDEREÇO, da aba DADOS PESSOAIS, deve conter a expressão "natal", restringindo o universo de seleção). Com oportunidade é possível ampliar o universo de seleção acresecentando aos critérios expressões como "parnamirim", "mipibu", "macaiba", "nisia" etc.  

