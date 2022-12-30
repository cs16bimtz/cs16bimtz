Sistema de Acompanhamento da Seleção Complementar - Guia do utilizador 👋

### 1 - INTRODUÇÃO AO SisASC
Seja bem vindo ao **Sistema de Acompanhamento da Seleção Complementar - SisASC/16º BI Mtz**. O SisASC é um instrumento de gestão e foi concebido para ser a ferramenta de coleta e processamento de dados dos conscritos durante a execução da seleção complementar na OM.

### 2 - COMPOSIÇÃO DO SisASC
O sistema é composto basicamente de um formulário de cadastro denominado **Ficha Digital de Entrevista (FDE)** cujos campos são os campos da Ficha de Entrevista do Conscrito nos moldes como a conhecemos. A FDE contempla um conjunto de abas ou grupos (`DADOS PESSOAIS`, `TÍTULO DE ELEITOR`, `CNH`, `EXAME MÉDICO`, `EXAME ODONTOLÓGICO`, `TESTE DE HABILIDADES`, `PERFIL SOCIOECONÔMICO`, etc). 

Em cada aba da FDE os campos de formulário foram agrupados respeitando a afinidade que os dados guardam entre si. 

Na FDE os campos que serão utilizados como critério de seleção possuem um tipo de validação (noempty) que impede que os mesmos sejam armazenados com valor NULL no banco de dados. São campos, portanto, de preenchimento obrigatório por parte do entrevistador.

A FDE tem inúmeras vantagens quando comparada à Ficha de Entrevista padrão:
- Abstração do uso de papel e de impressão ao longo de praticamente toda a realização da CS;
- Controle eficiente de todas fases da CS;
- Quase a totalidade dos campos da FDE são do tipo *dropdow* (botões com alternância de visibilidade de listas, também chamados de listas suspensas), *checkbox* (caixas de checagem) ou *radiobuton* (recurso que permite ao usuário selecionar apenas um ítem entre vários). A utilização desses recursos de formulário reduz drasticamente o tempo de entrevista/candidato em virtude da simplicidade, da rapidez no preenchimento e no processamento dos dados;
- Menu de opções: os menus agrupam, também por afinidade, as diversas consultas (relatórios) disponíveis no SisASC.

### 3 - APRESENTAÇÃO DAS ABAS (GRUPOS) DE DADOS:
<details>
<summary>:eyes: <kbd>DADOS PESSOAIS</kbd></summary>
 
![menus e abas 5](https://user-images.githubusercontent.com/121310141/209486078-dd89a412-65c7-4e53-bc3d-2db3ab8643e8.png)

 Na imagem acima temos a aba DADOS PESSOAIS da Ficha "Digital" de Entrevista do Conscrito em evidência. 
 > **Note**
> Repare que o sistema recusa o cadastramanto do conscrito se `quaisquer` dos campos: NOME, CPF, ESTADO CIVIL, RELIGIÃO, ESCOLARIDADE, VOLUNTÁRIO ou ENTREVISTADOR não forem corretamente preenchidos. 

> **Note**
> O campo CPF do formulário tem validação *isunique*, garantindo que cada CPF armazenado no banco de dados seja único. De outra forma: o sistema não permitirá a duplicidade de cadastro.  
</details>

<details>
<summary>:eyes: <kbd>INSPEÇÃO MÉDICA</kbd></summary>
 
![fm](https://user-images.githubusercontent.com/121310141/209503889-b8d7322c-934d-472d-895f-1b6718a2b76d.png)

Na imagem acima temos a aba DADOS PESSOAIS da Ficha "Digital" de Entrevista do Conscrito em evidência. 
 > **Note**
> Repare que o sistema recusa o cadastramanto do conscrito se `quaisquer` dos campos: NOME, CPF, ESTADO CIVIL, RELIGIÃO, ESCOLARIDADE, VOLUNTÁRIO ou ENTREVISTADOR não forem corretamente preenchidos. 

> **Note**
> O campo CPF do formulário tem validação *isunique*, garantindo que cada CPF armazenado no banco de dados seja único. De outra forma: o sistema não permitirá a duplicidade de cadastro.  
</details>
  
### 4 - CARACTERÍSTICAS DO SisASC
No SisASC os atributos/características desejáveis no conscrito (Perfil do Conscrito) são os parametros que foram configurados (setados) no sistema e que podem ser alterados a critéro do Cmt OM.

O sistema terá as configurações necessárias para garantir que todos os conscritos selecionados para a incorporação, atendam aos requisitos que a unidade deseja. 

Para que o conscrito seja considerado <kbd>indicado</kbd> na entrevista, uma série de requisitos devem ser satisfeitos; para que o conscrito seja <kbd>Contraindicado</kbd> na fase de entrevista, todavia, basta que apenas um dos parâmetros (requisitos) não seja atendido. Essas características do sistema garantem o rigor e a homogeneidade do processo seletivo. 

No entanto, se durante a fase de processamento dos dados (fase pós CS), o número necessário de conscritos para o preenchimento dos `claros` não tenha sido atingido, em virtude do rigor dos parâmetros definidos no sistema, a critério do Cmt OM, tais parâmetros podem ser flexibilizados obedecendo a uma precedência definida também pelo Cmt OM, sem prejuízo para o processo. Conclui-se daí que existe uma fase aonde são coletados os dados dos conscritos (dados pessoais, dados socioeconomicos, dados médicos, etc) e uma outra fase muita curta aonde os dados coletados são processados. 

Exemplo: O Cmt pode estabelecer inicialmente que todos os conscritos selecionados para a incorporação necessariamente devam residir em Natal (campo ENDEREÇO, da aba DADOS PESSOAIS, deve conter a expressão "natal", restringindo o universo de seleção). Com oprtunidade é possível ampliar o universo de seleção acresecentando aos critérios expressões como "parnamirim", "mipibu", "macaiba", "nisia" etc.  

> **Warning**
> A situação de contraindicado durante a fase de entrevista, depende da negação de apenas um dos parâmetros.

Principais características do **`SisASC/16º BI Mtz`**:

- Ferramenta de gestão e controle; 
- Ficha Digital de Entrevista (FDE); 
- Relatórios (Consultas) predefinidos no sistema: 
   - Indicados/Contraindicados na Entrevista;
   - Aptos/Inaptos na Inspeção de Saúde;
   - Voluntários/Não voluntários;
   - Possuem/Não possuem habilidades;
   - Classificados/Não classificados para a incorporação;
   - Outras consultas (Conscritos/Estado Civil, Conscritos/Escolaridade, Conscritos/Religião, etc...)  
- Ferramenta de busca avançada; 
- Impressão da Ficha de Entrevista gerada. 
- Imprime e exporta consulta PDF, CSV; 
- Formulário para cadastramento de entrevistadores 
- Controle de acesso; 
- Log de ações do usuário (auditoria); 

### 5 - TERMINOLOGIA/FASE DA `COMISSÃO DE SELEÇÃO` NO SisASC
|  Nº FASE |DESCRIÇÃO DA FASE|      CONFORME  |   NÃO CONFORME  |  OBS | 
|:--------:|-----------------|:--------------:|:---------------:|:----:|
|  1       | ENTREVISTA      |  INDICADO      | CONTRAINDICADO  |  -   | 
|  2       | EXAME MÉDICO    |  APTO          | INAPTO          |  -   |
|  3       | EXAME ODONTO    |  APTO          | INAPTO          |  -   | 
|  4       | TESTE HABILIDADE|  DEMONSTROU    | NÃO DEMONSTROU  |  -   | 
|  5       | INCORPORAÇÃO    |  CLASSIFICADO  | NÃO CLASSIFICADO|  -   | 

> **Note** 
> Na fase de entrevista o sistema adota os termos **indicado** e **contraindicado** para significar que o conscrito `atende/não atende` aos requisitos exigidos; ao longo da  inspeção médica e da inspeção odontológica os termos utilizados são **apto** e **inapto** para indicar que o conscrito `possui/não possui` as característica que se deseja em um soldado; na fase onde são verificadas as habilidades declaradas pelo conscrito na FDE, os termos utilizados são **demonstrou** e **não demonstrou** a competência declarada; na etapa onde são processados os dados coletados os termos utilizados são **classificado** e **não classificado** para indicar que o conscrito foi `selecionado/não selecionado` para a incorporação.

### 6 - PARÂMETROS DE CONFIGURAÇÃO UTILIZADOS NO SisASC:
#### Parametrização de alguns dos campos de formulário da aba `DADOS PESSOAIS`, para o conscrito ser considerado <kbd>Indicado</kbd> na fase 1 (ENTREVISTA) do processo seletivo:
 ABA DE DADOS DO FORMULÁRIO |            CAMPO DE FORMULÁRIO      |     CONDIÇÃO (CRITÉRIO OU PARÂMETRO UTILIZADO)     | STATUS   | OBS                          |
----------------------------|-------------------------------------|----------------------------------------------------|----------|------------------------------|
 DADOS PESSOAIS             | ESTADO CIVIL                        | Solteiro                                           | INDICADO |                              |
 DADOS PESSOAIS             | RELIGIÃO                            | !=Adventista                                       | INDICADO |Não pode ser adventista       |
 DADOS PESSOAIS             | ESCOLARIDADE                        | !=Ensino fundamental incompleto                    | INDICADO |Pelo menos o EF completo      |
 DADOS PESSOAIS             | VOLUNTÁRIO                          | Sim                                                | INDICADO |                              |
> **Note**
> No campo `RELIGIÃO` da aba DADOS PESSOAIS, se o valor selecionado for "Adventista", o conscrito será automaticamente contraindicado, independente de quais sejam as respostas para os demais campos utilizados como parâmetros na aba considerada. Lembre-se de que esse é um campo com validação (noempty). O entrevistador é impedido de salvar/cadastrar as demais informações do conscrito se esse campo não for preenchido.  

> **Note**
> Não existe no sistema o botão `Indicado`, ou `Indicar candidato`, ou `Indicar conscrito`. Essa tarefa foi automatizada, significando dizer que o próprio sistema se encarregará de indicar (ou contraindicar) o conscrito a partir dos dados coletados na FDE em confronto com os parâmetros configurados.

#### Parametrização de alguns dos campos de formulário da aba `PERFIL SOCIOECONÔMICO` para o conscrito ser considerado <kbd>Indicado</kbd> ainda na fase 1 (ENTREVISTA) do processo seletivo:
 ABA DE DADOS DO FORMULÁRIO |            CAMPO DE FORMULÁRIO      |     CONDIÇÃO (CRITÉRIO OU PARÂMETRO UTILIZADO)     | STATUS   | OBS                          |
----------------------------|-------------------------------------|----------------------------------------------------|----------|------------------------------|
 PERFIL SOCIOECONÔMICO      | MORA COM QUEM NO ENDEREÇO DECLARADO | Pais                                               | INDICADO |                              |
 PERFIL SOCIOECONÔMICO      | EM CASO DE CONVOCAÇÃO               | !=Adotarei o aquartelamento como residência        | INDICADO |Não pode querer ser laranjeira|
 PERFIL SOCIOECONÔMICO      | ARRIMO DE FAMÍLIA                   | Não                                                | INDICADO |                              |
 PERFIL SOCIOECONÔMICO      | PASSAGEM PELA POLÍCIA               | Não                                                | INDICADO |                              |
 PERFIL SOCIOECONÔMICO      | EXPERIÊNCIA COM DROGAS              | Não                                                | INDICADO |                              |
 PERFIL SOCIOECONÔMICO      | USO DE ARMA DE FOGO                 | Não                                                | INDICADO |                              |
> **Note**
> No campo denominado `MORA COM QUEM NO ENDEREÇO DECLARADO` da aba PERFIL SOCIOECONÔMICO, se o valor selecionado for diferente (!=) de "Pais", o conscrito será automaticamente contraindicado, independente de quais sejam as respostas para os demais campos utilizados como parâmetros na aba considerada. Repare que os critérios podem ser tão rigorosos quanto possível. Nesse batalhão hipotético todos os conscritos devem morar com os pais, porque morar com os pais pressupõe que o candidato seja detentor de valores morais e éticos que só podem ser adquiridos com a convivência em um grupo familiar, valores esses, essenciais à vida na caserna.

#### Parametrização de alguns dos campos de formulário da aba `EXAME MÉDICO` para o conscrito ser considerado <kbd>Apto</kbd> na fase 2 (EXAME MÉDICO) do processo seletivo:
 ABA DE DADOS DO FORMULÁRIO |            CAMPO DE FORMULÁRIO      |     CONDIÇÃO (CRITÉRIO OU PARÂMETRO UTILIZADO)     | STATUS   | OBS                          |
----------------------------|-------------------------------------|----------------------------------------------------|----------|------------------------------|
 EXAME MÉDICO               | TOMA REMÉDIO CONTROLADO             | Não                                                | APTO     |                              |
 EXAME MÉDICO               | FEZ OU FAZ                          | !=Tratamento Psicológico                           | APTO     |                              |
 EXAME MÉDICO               | FEZ OU FAZ                          | !=Tratamento Psiquiátrico                          | APTO     |                              |

#### Parametrização de alguns dos campos de formulário da aba `EXAME ODONTOLÓGICO` para o conscrito ser considerado <kbd>Apto</kbd> na fase 3 (EXAME ODONTO) do processo seletivo:
 ABA DE DADOS DO FORMULÁRIO |            CAMPO DE FORMULÁRIO      |     CONDIÇÃO (CRITÉRIO OU PARÂMETRO UTILIZADO)     | STATUS   | OBS                          |
----------------------------|-------------------------------------|----------------------------------------------------|----------|------------------------------|
 EXAME ODONTO               | QNT DE CÁRIE DE ESMALTE             | <=3  (por exemplo)                                 | APTO     |                              |
 EXAME ODONTO               | QNT DE CÁRIE DE DENTINA             | <=3  (por exemplo)                                 | APTO     |                              |
 EXAME ODONTO               | QNT RESTAURAÇÕES INADEQUADAS        | <=3  (por exemplo)                                 | APTO     |                              |
 EXAME ODONTO               | QNT AUSÊNCIA DENT ANTERIOR          | <=3  (por exemplo)                                 | APTO     |                              |
 EXAME ODONTO               | QNT AUSÊNCIA DENT POSTERIOR         | <=3  (por exemplo)                                 | APTO     |                              |

> **Note**
> Não existe também no sistema, na fase de realização dos exames médicos/adontológicos, o botão `Apto`, ou `Conscrito apto`, ou `Conscrito inapto`. Essa tarefa também foi automatizada, significando dizer que o próprio sistema se encarregará de definir se o conscrito foi apto (ou inapto), a partir dos dados coletados na FDE em confronto com os parâmetros configurados, que por enquanto são os constantes das tabelas acima.

### 7 - STATUS DO CONSCRITO AO FINAL DA SELEÇÃO/CASO (1-5)
|  CASO |ENTREVISTA|EXAME MÉDICO|EXAME ODONTO|TESTE DE HABILIDADES|  STATUS | OBS|
| :-----: | :--------: | :----------: | :----------: | :------------------: | :-------: | :-----: |
| 1     |      🟢  |     🟢    |      🟢    |              🟢  | CLASSIFICADO |    |
| 2     |      🟢  |     🟢    |      🟢    |               🔴  |   CLASSIFICADO|    |
| 3     |      🟢  |     🟢    |      🔴    |                    |  NÃO CLASSIFICADO |    |
| 4     |      🟢  |     🔴    |             |                   | NÃO CLASSIFICADO    |    |
| 5     |      🔴  |            |            |                    |   NÃO CLASSIFICADO   |   | 

> **Note**
> Conscrito contraindicado na entrevista não realiza a fase seguinte conforme Caso 5 da tabela STATUS/CASO.

> **Note**
> Conscrito `Não conforme` em uma das fases não realiza a triagem na fase seguinte (Casos 3, 4 e 5). 

### 8 - TABELA DE USUÁRIOS DO SISTEMA
|     Nº   |        NOME DO UTILIZADOR        |      USUÁRIO     |      SENHA      |  OBS | 
|:--------:|----------------------------------| :--------------: | :-------------: | :---:|
|  1       | Presidente da CS                 |            chcs  |       root      |  -   | 
|  2       | Médico 1                         |         medico_1 |       root      |  -   |
|  3       | Médico 2                         |         medico_2 |       root      |  -   | 
|  4       | Dentista                         |       dentista_1 |       root      |  -   | 
|  5       | Entrevistador 1                  |  entrevistador_1 |       root      |  -   | 
|  6       | Entrevistador 2                  |  entrevistador_2 |       root      |  -   | 
|  7       | Entrevistador 3                  |  entrevistador_3 |       root      |  -   | 
|  8       | Entrevistador 4                  |  entrevistador_4 |                 |  -   | 
|  9       | Entrevistador 5                  |  entrevistador_5 |                 |  -   | 
|  10      | Entrevistador 6                  |  entrevistador_6 |                 |  -   | 
> **Note**
> As senhas serão redefinidas por ocasião da CS; 

> **Note**
> Cada entevistador tem visibilidade apenas dos seus entrevistados

> **Note**
> Os critérios para a classificação do conscrito no processo seletivo, embora pareçam óbvios não são de inteiro conhecimento do entrevistador. 

### 9 - TABELA DE PERMISSÕES
|  Nº |      PERFIL       | DADOS PESSOAIS |TITULO ELEITOR|CNH|EXAME MÉDICO|EXAME ODONTO|TESTE HABILIDADES|PERFIL SOCIOECONOMICO|  OBS |
|:---:|-------------------|:--------------:|:------------:|:-:|:----------:|:----------:|:---------------:|:-------------------:|:----:|
|  1  | Cmt OM            | ALL            | ALL          |ALL| ALL        |ALL         | ALL             | ALL                 | -    |
|  2  | Presidente da CS  | ALL            | ALL          |ALL| ALL        |ALL         | ALL             | ALL                 | -    |
|  3  | Médico            |V               | V            |V  | IEV        |V           | V               | V                   | -    |
|  4  | Dentista          |V               | V            |V  | V          |IEV         | V               | V                   | -    |
|  5  | Entrevistador     | ALL            | ALL          |ALL| V          |V           | ALL             | ALL                 | -    |









## 5 - TABELA DE PERMISSÕES
<table class="table table-striped" style="width: 1187px;">
<thead>
<tr style="height: 15px;">
<th style="width: 1144.09px; height: 15px;">Seção</th>
<th style="width: 10px; height: 15px;">User </th>
<th style="width: 674px; height: 15px;">Password</th>
<th style="width: 621px; text-align: center; height: 15px;"> Create</th>
<th style="width: 830px; text-align: center; height: 15px;"> Read</th>
<th style="width: 723px; text-align: center; height: 15px;"> Update</th>
<th style="width: 578px; text-align: center; height: 15px;">Delete </th>
<th style="width: 1153px; text-align: center; height: 15px;">Disable record</th>
<th style="width: 961px; text-align: center; height: 15px;">Enable record</th>
</tr>
</thead>
<tbody>
<tr style="height: 15px;">
<td style="width: 1144.09px; height: 15px; text-align: left;">Super user</td>
<td style="width: 10px; height: 15px;"> root</td>
<td style="width: 674px; height: 15px;">root</td>
<td style="width: 621px; height: 15px; text-align: left;">x </td>
<td style="width: 830px; height: 15px; text-align: left;">x </td>
<td style="width: 723px; height: 15px; text-align: left;">x </td>
<td style="width: 578px; height: 15px; text-align: left;">x</td>
<td style="width: 1153px; height: 15px; text-align: left;">x </td>
<td style="width: 961px; height: 15px; text-align: left;">x</td>
</tr>
<tr style="height: 15px;">
<td style="width: 1144.09px; height: 15px; text-align: left;">Cmt 16º BI Mtz</td>
<td style="width: 10px; height: 15px;"> cmtom</td>
<td style="width: 674px; height: 15px;">root</td>
<td style="width: 621px; height: 15px; text-align: left;">x</td>
<td style="width: 830px; height: 15px; text-align: left;">x</td>
<td style="width: 723px; height: 15px; text-align: left;">x</td>
<td style="width: 578px; height: 15px; text-align: left;">x</td>
<td style="width: 1153px; height: 15px; text-align: left;">x</td>
<td style="width: 961px; height: 15px; text-align: left;"> </td>
</tr>
<tr style="height: 15px;">
<td style="width: 1144.09px; height: 15px;">1ª Seção</td>
<td style="width: 10px; height: 15px;"> ch1secao</td>
<td style="width: 674px; height: 15px;">root</td>
<td style="width: 621px; height: 15px; text-align: left;">x</td>
<td style="width: 830px; height: 15px; text-align: left;">x</td>
<td style="width: 723px; height: 15px; text-align: left;">x</td>
<td style="width: 578px; height: 15px; text-align: left;">x </td>
<td style="width: 1153px; height: 15px; text-align: left;">x</td>
<td style="width: 961px; height: 15px; text-align: left;"> </td>
</tr>
<tr style="height: 15px;">
<td style="width: 1144.09px; height: 15px;">2ª Seção</td>
<td style="width: 10px; height: 15px;"></td>
<td style="width: 674px; height: 15px;"></td>
<td style="width: 621px; height: 15px; text-align: left;"></td>
<td style="width: 830px; height: 15px; text-align: left;"></td>
<td style="width: 723px; height: 15px; text-align: left;"></td>
<td style="width: 578px; height: 15px; text-align: left;"></td>
<td style="width: 1153px; height: 15px; text-align: left;"></td>
<td style="width: 961px; height: 15px; text-align: left;"></td>
</tr>
<tr style="height: 15px;">
<td style="width: 1144.09px; height: 15px; text-align: left;">3ª Seção</td>
<td style="width: 10px; height: 15px;"></td>
<td style="width: 674px; height: 15px;"></td>
<td style="width: 621px; height: 15px; text-align: left;"></td>
<td style="width: 830px; height: 15px; text-align: left;"></td>
<td style="width: 723px; height: 15px; text-align: left;"></td>
<td style="width: 578px; height: 15px; text-align: left;"></td>
<td style="width: 1153px; height: 15px; text-align: left;"></td>
<td style="width: 961px; height: 15px; text-align: left;"></td>
</tr>
<tr style="height: 15px;">
<td style="width: 1144.09px; height: 15px; text-align: left;">1ª Cia Fuz</td>
<td style="width: 10px; height: 15px;"> cmt1ciafuz</td>
<td style="width: 674px; height: 15px;">root</td>
<td style="width: 621px; height: 15px; text-align: left;">x</td>
<td style="width: 830px; height: 15px; text-align: left;">x</td>
<td style="width: 723px; height: 15px; text-align: left;">x</td>
<td style="width: 578px; height: 15px; text-align: left;"> </td>
<td style="width: 1153px; height: 15px; text-align: left;">x</td>
<td style="width: 961px; height: 15px; text-align: left;"> </td>
</tr>
<tr style="height: 15px;">
<td style="width: 1144.09px; height: 15px; text-align: left;">1ª Cia Fuz</td>
<td style="width: 10px; height: 15px;"> sgte1ciafuz</td>
<td style="width: 674px; height: 15px;">root</td>
<td style="width: 621px; height: 15px; text-align: left;">x</td>
<td style="width: 830px; height: 15px; text-align: left;">x</td>
<td style="width: 723px; height: 15px; text-align: left;">x</td>
<td style="width: 578px; height: 15px; text-align: left;"> </td>
<td style="width: 1153px; height: 15px; text-align: left;">x</td>
<td style="width: 961px; height: 15px; text-align: left;"> </td>
</tr>
<tr style="height: 16.4583px;">
<td style="width: 1144.09px; height: 16.4583px; text-align: left;">2ª Cia Fuz</td>
<td style="width: 10px; height: 16.4583px; text-align: left;">cmt2ciafuz</td>
<td style="width: 674px; height: 16.4583px;">root</td>
<td style="width: 621px; height: 16.4583px; text-align: left;">x</td>
<td style="width: 830px; height: 16.4583px; text-align: left;">x</td>
<td style="width: 723px; height: 16.4583px; text-align: left;">x</td>
<td style="width: 578px; height: 16.4583px; text-align: left;"> </td>
<td style="width: 1153px; height: 16.4583px; text-align: left;">x</td>
<td style="width: 961px; height: 16.4583px; text-align: left;"> </td>
</tr>
<tr style="height: 15px;">
<td style="width: 1144.09px; height: 15px; text-align: left;">2ª Cia Fuz</td>
<td style="width: 10px; height: 15px;"><kbd>sgte2ciafuz</kbd></td>
<td style="width: 674px; height: 15px;">root</td>
<td style="width: 621px; height: 15px; text-align: left;">x</td>
<td style="width: 830px; height: 15px; text-align: left;">x </td>
<td style="width: 723px; height: 15px; text-align: left;">x </td>
<td style="width: 578px; height: 15px; text-align: left;"> </td>
<td style="width: 1153px; height: 15px; text-align: left;">x</td>
<td style="width: 961px; height: 15px; text-align: left;"> </td>
</tr>
<tr style="height: 15px;">
<td style="width: 1144.09px; height: 15px; text-align: left;">Cia C Ap</td>
<td style="width: 10px; height: 15px;"> cmtciacap</td>
<td style="width: 674px; height: 15px;">root</td>
<td style="width: 621px; height: 15px; text-align: left;">x </td>
<td style="width: 830px; height: 15px; text-align: left;">x </td>
<td style="width: 723px; height: 15px; text-align: left;">x </td>
<td style="width: 578px; height: 15px; text-align: left;"> </td>
<td style="width: 1153px; height: 15px; text-align: left;">x </td>
<td style="width: 961px; height: 15px; text-align: left;"> </td>
</tr>
<tr style="height: 15px;">
<td style="width: 1144.09px; height: 15px; text-align: left;">Cia C Ap</td>
<td style="width: 10px; height: 15px;"> sgteciacap</td>
<td style="width: 674px; height: 15px;">root</td>
<td style="width: 621px; height: 15px; text-align: left;">x </td>
<td style="width: 830px; height: 15px; text-align: left;">x </td>
<td style="width: 723px; height: 15px; text-align: left;">x </td>
<td style="width: 578px; height: 15px; text-align: left;"> </td>
<td style="width: 1153px; height: 15px; text-align: left;">x </td>
<td style="width: 961px; height: 15px; text-align: left;"> </td>
</tr>
<tr style="height: 15px;">
<td style="width: 1144.09px; height: 15px; text-align: left;">NPOR</td>
<td style="width: 10px; height: 15px;"> instrchnpor</td>
<td style="width: 674px; height: 15px;">root</td>
<td style="width: 621px; height: 15px; text-align: left;">x</td>
<td style="width: 830px; height: 15px; text-align: left;">x </td>
<td style="width: 723px; height: 15px; text-align: left;">x</td>
<td style="width: 578px; height: 15px; text-align: left;"> </td>
<td style="width: 1153px; height: 15px; text-align: left;">x </td>
<td style="width: 961px; height: 15px; text-align: left;"> </td>
</tr>
  <tr style="height: 15px;">
<td style="width: 1144.09px; height: 15px; text-align: left;">NPOR</td>
<td style="width: 10px; height: 15px;"> instr1npor</td>
<td style="width: 674px; height: 15px;">root</td>
<td style="width: 621px; height: 15px; text-align: left;">x</td>
<td style="width: 830px; height: 15px; text-align: left;">x </td>
<td style="width: 723px; height: 15px; text-align: left;">x</td>
<td style="width: 578px; height: 15px; text-align: left;"> </td>
<td style="width: 1153px; height: 15px; text-align: left;">x </td>
<td style="width: 961px; height: 15px; text-align: left;"> </td>
</tr>
  <tr style="height: 15px;">
<td style="width: 1144.09px; height: 15px; text-align: left;">NPOR</td>
<td style="width: 10px; height: 15px;"> instr2npor</td>
<td style="width: 674px; height: 15px;">root</td>
<td style="width: 621px; height: 15px; text-align: left;">x</td>
<td style="width: 830px; height: 15px; text-align: left;">x </td>
<td style="width: 723px; height: 15px; text-align: left;">x</td>
<td style="width: 578px; height: 15px; text-align: left;"> </td>
<td style="width: 1153px; height: 15px; text-align: left;">x </td>
<td style="width: 961px; height: 15px; text-align: left;"> </td>
</tr>
<tr style="height: 15px;">
<td style="width: 1144.09px; height: 15px; text-align: left;">NPOR</td>
<td style="width: 10px; height: 15px;"> sgtenpor</td>
<td style="width: 674px; height: 15px;">root</td>
<td style="width: 621px; height: 15px; text-align: left;">x </td>
<td style="width: 830px; height: 15px; text-align: left;">x </td>
<td style="width: 723px; height: 15px; text-align: left;">x </td>
<td style="width: 578px; height: 15px; text-align: left;"> </td>
<td style="width: 1153px; height: 15px; text-align: left;">x </td>
<td style="width: 961px; height: 15px; text-align: left;"> </td>
</tr>
<tr style="height: 15px;">
<td style="width: 1144.09px; height: 15px; text-align: left;">CFGS</td>
<td style="width: 10px; height: 15px;"> instrchcfgs</td>
<td style="width: 674px; height: 15px;">root</td>
<td style="width: 621px; height: 15px; text-align: left;">x </td>
<td style="width: 830px; height: 15px; text-align: left;">x </td>
<td style="width: 723px; height: 15px; text-align: left;">x </td>
<td style="width: 578px; height: 15px; text-align: left;"> </td>
<td style="width: 1153px; height: 15px; text-align: left;">x </td>
<td style="width: 961px; height: 15px; text-align: left;"> </td>
</tr>
<tr style="height: 15px;">
<td style="width: 1144.09px; height: 15px; text-align: left;">CFGS</td>
<td style="width: 10px; height: 15px;"> sgtecfgs</td>
<td style="width: 674px; height: 15px;">root</td>
<td style="width: 621px; height: 15px; text-align: left;">x</td>
<td style="width: 830px; height: 15px; text-align: left;">x</td>
<td style="width: 723px; height: 15px; text-align: left;">x</td>
<td style="width: 578px; height: 15px; text-align: left;"> </td>
<td style="width: 1153px; height: 15px; text-align: left;">x</td>
<td style="width: 961px; height: 15px; text-align: left;"> </td>
</tr>
  <tr style="height: 15px;">
<td style="width: 1144.09px; height: 15px; text-align: left;">B Mus</td>
<td style="width: 10px; height: 15px;"> sgtebanda</td>
<td style="width: 674px; height: 15px;">root</td>
<td style="width: 621px; height: 15px; text-align: left;">x</td>
<td style="width: 830px; height: 15px; text-align: left;">x</td>
<td style="width: 723px; height: 15px; text-align: left;">x</td>
<td style="width: 578px; height: 15px; text-align: left;"> </td>
<td style="width: 1153px; height: 15px; text-align: left;">x</td>
<td style="width: 961px; height: 15px; text-align: left;"> </td>
</tr>
</tbody>
</table>
