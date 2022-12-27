Sistema de Acompanhamento da Seleção Complementar - Guia do utilizador 👋

### 1 - INTRODUÇÃO AO SisASC
Seja bem vindo ao **Sistema de Acompanhamento da Seleção Complementar - SisASC/16º BI Mtz**. O SisASC é um instrumento de gestão e foi concebido para ser a ferramenta de coleta e processamento ou análise de dados dos conscritos durante a execução da seleção complementar na OM.

### 2 - COMPOSIÇÃO DO SisASC
O sistema é composto basicamente de um formulário de cadastro denominado **Ficha Digital de Entrevista (FDE)** cujos campos são os campos da Ficha de Entrevista do Conscrito nos moldes como a conhecemos. A FDE contempla um conjunto de abas ou grupos (`DADOS PESSOAIS`, `TÍTULO DE ELEITOR`, `CNH`, `INSPEÇÃO MÉDICA`, `INSPEÇÃO ODONTOLÓGICA`, `TESTE DE HABILIDADES`, `PERFIL SOCIOECONÔMICO`, etc). 

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

O sistema possui as configurações necessárias para garantir que todos os conscritos selecionados para a incorporação, atendam aos requisitos que a unidade deseja. Para que o conscrito seja considerado <kbd>indicado</kbd> na entrevista, uma série de requisitos devem ser satisfeitos; para que o conscrito seja <kbd>Contraindicado</kbd> na fase de entrevista, todavia, basta que apenas um dos parâmetros (requisitos) não seja atendido. Essas características do sistema garantem o rigor e a homogeneidade do processo seletivo. 

No entanto se o número necessário de conscritos para o preenchimento dos `claros` não for atingido, a critério do Cmt OM, os parâmerros podem ser flexibilizados obedecendo a uma precedência definida pelo Cmt OM. Conclui-se daí que existe uma fase aonde são coletados os dados dos conscritos (dados pessoais, dados socioeconomicos, dados médicos, etc) e uma outra fase muita curta aonde os dados coletados são processados. 
> **Note**
> Não existe no sistema o botão `Indicado`, ou `indicar candidato`, ou `Indicar conscrito`. Essa tarefa foi automatizada, significando dizer que o próprio sistema se encarregará de indicar (ou contraindicar) o conscrito a partir dos dados coletados na FDE em confronto com os parâmetros configurados.

> **Warning**
> A situação de contraindicado durante a fase de entrevista, depende da negação de apenas um dos parâmetros.

Principais características do **`SisASC/16º BI Mtz`**:

- Ferramenta de gestão e controle; 
- Ficha Digital de Entrevista (FDE); 
- Relatórios (Consultas) predefinidos no sistema: 
   - Indicados/contraindicados na entrevista;
   - Aptos/inaptos na inspeção de saúde;
   - Voluntários/não voluntários;
   - Possuem/não possuem habilidades;
   - Classificados/não classificados para a incorporação;
- Ferramenta de busca avançada; 
- Impressão da Ficha de Entrevista gerada. 
- Imprime e exporta consulta PDF, CSV; 
- Formulário para cadastramento de entrevistadores 
- Controle de acesso; 
- Log de ações do usuário (auditoria); 

### 5 - TERMINOLOGIA UTILIZADA NO SisASC
 DESCRIÇÃO DA FASE/TERMO UTILIZADO |   CONFORME   |   NÃO CONFORME   | 
-----------------------------------|--------------|------------------|
 Entrevista                        | Indicado     | Contraindicado   |   
 Inspeção médica                   | Apto         | Inapto           |      
 Inspeção odonto                   | Apto         | Inapto           |      
 Teste habilidades                 | Demonstrou   | Não demonstrou   |      
 Incorporação                      | Classificado | Não clasiificado |      
 
> **Note** 
> Na fase de entrevista o sistema adota os termos **indicado** e **contraindicado** para significar que o conscrito atende/não atende aos requisitos exigidos; ao longo da  inspeção médica e da inspeção odontológica os termos utilizados são **apto** e **inapto** para indicar que o conscrito possui/não possui as característica que se deseja em um soldado; na fase onde são verificadas as habilidades declaradas pelo conscrito na FDE, os termos utilizados são **demonstrou** e **não demonstrou** a competência declarada; na etapa onde são processados os dados coletados os termos utilizados são **classificado** e **não classificado** para indicar que o conscrito foi selecionado/não selecionado para a incorporação.

## 6 - PARÂMETROS DE CONFIGURAÇÃO UTILIZADOS NO SisASC:
Parametrização dos campos de formulário das abas DADOS PESSOAIS e PERFIL SOCIOECONÔMICO para o conscrito ser considerado indicado na entrevista:
 ABA DE DADOS DO FORMULÁRIO |            CAMPO DE FORMULÁRIO      |                    CRITÉRIO UTILIZADO              | STATUS   | OBS                          |
----------------------------|-------------------------------------|----------------------------------------------------|----------|------------------------------|
 DADOS PESSOAIS             | ESTADO CIVIL                        | Solteiro                                           | INDICADO |                              |
 DADOS PESSOAIS             | RELIGIÃO                            | &lt;&gt; Adventista                                | INDICADO |Não pode ser adventista       |
 DADOS PESSOAIS             | ESCOLARIDADE                        | &lt;&gt; Ensino fundamental incompleto             | INDICADO |Pelo menos o EF completo      |
 DADOS PESSOAIS             | VOLUNTÁRIO                          | Sim                                                | INDICADO |                              |
 PERFIL SOCIOECONÔMICO      | MORA COM QUEM NO ENDEREÇO DECLARADO | Pais                                               | INDICADO |                              |
 PERFIL SOCIOECONÔMICO      | EM CASO DE CONVOCAÇÃO               | &lt;&gt; Adotarei o aquartelamento como residência | INDICADO |Não pode querer ser laranjeira|
 PERFIL SOCIOECONÔMICO      | ARRIMO DE FAMÍLIA                   | Não                                                | INDICADO |                              |
 PERFIL SOCIOECONÔMICO      | PASSAGEM PELA POLÍCIA               | Não                                                | INDICADO |                              |
 PERFIL SOCIOECONÔMICO      | EXPERIÊNCIA COM DROGAS              | Não                                                | INDICADO |                              |
 PERFIL SOCIOECONÔMICO      | USO DE ARMA DE FOGO                 | Não                                                | INDICADO |                              |

> **Note**
> No campo `RELIGIÃO` da aba DADOS PESSOAIS, se o valor selecionado for "Adventista", o conscrito será automaticamente contraindicado, independente de quais sejam as respostas para os demais campos utilizados como parâmetros na aba considerada.

> **Note**
> No campo denominado `MORA COM QUEM NO ENDEREÇO DECLARADO` da aba PERFIL SOCIOECONÔMICO, se o valor selecionado for diferente de "Pais", o conscrito será automaticamente contraindicado, independente de quais sejam as respostas para os demais campos utilizados como parâmetros na aba considerada. Repare que os critérios podem ser tão rigorososo quanto possível. Nesse batalhão hipotético todos os candidatos devem moram com os pais, porque morar com os pais presupõe certos valores morais e éticos. Sabemos que essa premissa pode não ser sempre verdadeira.


## 7 - RESULTADO/FASE DA SELEÇÃO
<table style="width: 100%; height: 109px; border-color: #000000;" border="1"r>
<tbody>
<tr>
<td style="text-align: center;"><strong>CASO</strong></td>
<td style="text-align: center;"><strong>ENTREVISTA</strong></td>
<td style="text-align: center;"><strong>INSPEÇÃO MÉDICA</strong></td>
<td style="text-align: center;"><strong>INSPEÇÃO ODONTO</strong></td>
<td style="text-align: center;"><strong>TESTE DE HABILIDADES</strong></td>
<td style="text-align: center;"><strong>STATUS</strong></td>
</tr>
<tr>
<td style="text-align: center;"><strong>1</strong></td>
<td style="text-align: center;"><strong>🟢</strong></td>
<td style="text-align: center;"><strong>🟢</strong></td>
<td style="text-align: center;"><strong>🟢</strong></td>
<td style="text-align: center;"><strong>🟢</strong></td>
<td style="text-align: center;"><strong>CLASSIFICADO</strong></td>
</tr>
<tr>
<td style="text-align: center;"><strong>2</strong></td>
<td style="text-align: center;"><strong>🟢</strong></td>
<td style="text-align: center;"><strong>🟢</strong></td>
<td style="text-align: center;"><strong>🟢</strong></td>
<td style="text-align: center;"><strong>🔴</strong></td>
<td style="text-align: center;"><strong>CLASSIFICADO</strong></td>
</tr>
<tr>
<td style="text-align: center;"><strong>3</strong></td>
<td style="text-align: center;"><strong>🟢</strong></td>
<td style="text-align: center;"><strong>🟢</strong></td>
<td style="text-align: center;"><strong>🔴</strong></td>
<td style="text-align: center;"><strong></strong></td>
<td style="text-align: center;"><strong>NÃO CLASSIFICADO</strong></td>
</tr>
<tr>
<td style="text-align: center;"><strong>4</strong></td>
<td style="text-align: center;"><strong>🟢</strong></td>
<td style="text-align: center;"><strong>🔴</strong></td>
<td style="text-align: center;"><strong></strong></td>
<td style="text-align: center;"><strong></strong></td>
<td style="text-align: center;"><strong>NÃO CLASSIFICADO</strong></td>
</tr>
<tr>
<td style="text-align: center;"><strong>5</strong></td>
<td style="text-align: center;"><strong>🔴</strong></td>
<td style="text-align: center;"><strong></strong></td>
<td style="text-align: center;"><strong></strong></td>
<td style="text-align: center;"><strong></strong></td>
<td style="text-align: center;"><strong>NÃO CLASSIFICADO</strong></td>
</tr>
</tbody>
</table>
## 8 - CONCEPÇÃO DE UMA SC UTILIZANDO O SisASC:
>**Note**
>Unicos candidatos dispensados em definitivo serão os `não voluntários` após passarem pela entrevista (entrevista apenas) no percentual de no máximo 50% do número de candidatos/dia.&nbsp. Lembre-se de que conforme a tabela de parâmetros o sistema se encarregará de contraindicar o candidato não voluntário.

>**Note**
> Candidato mal sucedido (contraindicado na entrevista, inapto no caso das inspeções médica e odontológica), não realiza a triagem na fase seguinte. 

>**Warning**
> Não há a hipóteses de o candidato sendo liberado sem passar pelo entrevistador.

>**Note**
> Prioridade na seana 15 a 19 de janeiro a coleta rigorosa de dados com suporte à tomada de decisão; Análise dos dados coletados na semana de 22 a 26.

 ### Exemplo
Para o candidato ser considerado **indicado** na fase de entrevista, os parâmetros inseridos no sistema foram os seguinte:
 - Na aba **DADOS PESSOAIS**

 Campo/parâmetro   | Indicado      | Contraindicado | 
-------------------|---------------|----------------|
 Voluntário  ✔️   | Sim           |                |   
 Estado civil      | Solteiro      |                |      
 Religião          | <> Adventista |                |   
 

 
 
