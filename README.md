Sistema de Acompanhamento da Seleção Complementar 👋

## INTRODUÇÃO
Seja bem vindo ao **Sistema de Acompanhamento da Seleção Complementar - SisASC/16º BI Mtz**. O SisASC é um instrumento de gestão e controle e foi concebido para ser a ferramenta de coleta de dados dos conscritos durante a execução da seleção complementar na OM.

## COMPOSIÇÃO
O sistema é composto basicamente de uma **Ficha de Entrevista (Digital)** e de um **Menu de opções**. 
 - Ficha Digital de Entrevista (FDE): é composta por um conjunto de abas (DADOS PESSOAIS, TÍTULO DE ELEITOR, CNH, INSPEÇÃO MÉDICA, INSPEÇÃO ODONTOLÓGICA, TESTE DE HABILIDADES, PERFIL SOCIOECONÔMICO, ETC). Em cada aba da FDE os campos de formulário foram agrupados respeitando a afinidade que os dados guardam entre si.
 - Menu de opções: os menus agrupam, também por afinidade, as diversas consultas (relatórios) disponíveis no SisASC.

![menus e abas 1](https://user-images.githubusercontent.com/121310141/209476833-cc7f8c83-6f32-494e-a391-2d6f78e0b27c.png)

Na imagem acima temos a aba DADOS PESSOAIS em evidência. 

Repare que o sistema recusa o cadastramanto do conscrito se os campos NOME, CPF, ESTADO CIVIL, RELIGIÃO, ESCOLARIDADE, e ENTREVISTADOR não forem corretamente preenchidos. O campo CPF do formulário tem validação "isunique", garantindo que cada CPF armazenado no banco de dados seja único. De outra forma, o sistema não permitirá a duplicidade de cadastro.  

  
## CARACTERÍSTICAS
No SisASC os atributos/características desejáveis no conscrito (Perfil do Candidato) são os parametros que foram configurados no sistema e que podem ser alterados a critéro do Cmt OM.

O sistema possui as configurações necessárias para garantir que todos os conscritos selecionados para a incorporação, atendam aos requisitos que a unidade deseja. Para que o conscrito seja considerado indicado na entrevista, uma série de requisitos devem ser satisfeitos; para que o conscrito seja contraindicado na fase de entrevista, todavia, basta que apenas um dos parâmetros (requisitos) não seja atendido. Essas características do sistema garantem o rigor e a homogeneidade do processo seletivo. 

No entanto se o número necessário de conscritos para o preenchimento dos "claros" não for atingido, a critério do Cmt OM, os parâmerros podem ser flexibilizados obedecendo a uma precedência definida pelo Cmt OM. 
> Não existe no sistema o botão "Indicado", ou "indicar candidato", ou "indicar conscrito". Essa tarefa foi automatizada, significando dizer que o próprio sistema se encarregará de indicar (ou contraindicar) o conscrito a partir dos dados coletados na FDE em confronto com os parâmetros configurados.

> **Note**
> Não existe no sistema o botão `Indicado`, ou `indicar candidato`, ou `ndicar conscrito`. Essa tarefa foi automatizada, significando dizer que o próprio sistema se encarregará de indicar (ou contraindicar) o conscrito a partir dos dados coletados na FDE em confronto com os parâmetros configurados.

> **Warning**
> A situação de contraindicado durante a fase de entrevista, depende da negação de apenas um dos parâmetros.

**Exemplo**: no campo RELIGIÃO da aba DADOS PESSOAIS, se o valor selecionado for "Adventista", o conscrito será automaticamente contraindicado independente de quais sejam as respostas para os demais campos utilizados como parâmetros.

Principais características do SisASC/16º BI Mtz:

✔️ Ferramenta de gestão e controle;
 
✔️ Ficha Digital de Entrevista (FDE);
 
✔️ Relatórios (Consultas) predefinidos no sistema:
 
   - Indicados/contraindicados na entrevista;
   - Aptos/inaptos na inspeção de saúde;
   - Voluntários/não voluntários;
   - Possuem/não possuem habilidades;
   - Classificados/não classificados para a incorporação;
 
✔️ Ferramenta de busca avançada;
 
✔️ Impressão da Ficha de Entrevista gerada.
 
✔️ Imprime e exporta consulta PDF, CSV;
 
✔️ Formulário para cadastramento de entrevistadores
 
✔️ Controle de acesso;
 
✔️ Log de ações do usuário (auditoria);
 

## TERMINOLOGIA:
 DESCRIÇÃO DA FASE/TERMO UTILIZADO | BEM SUCEDIDO |   MAL SUCEDIDO   | 
-----------------------------------|--------------|------------------|
 Entrevista                        | Indicado     | Contraindicado   |   
 Inspeção médica                   | Apto         | Inapto           |      
 Inspeção odonto                   | Apto         | Inapto           |      
 Teste habilidades                 | Demonstrou   | Não demonstrou   |      
 Incorporação                      | Classificado | Não clasiificado |      
 
Na fase de entrevista o sistema adota os termos **indicado** e **contraindicado** para significar que o conscrito foi bem ou mal sucedido durante essa etapa do processo; na fase de inspeção médica e odontológica os termos utilizados são **apto** e **inapto** para inddicar que o conscrito foi bem ou mal sucedido nessa fase da seleção de pessoal; na fase onde são verificadas as habilidades declaradas pelo conscrito, os termos utilizados são **demonstrou** e **não demonstrou** a competência declarada; na última etapa da seleçãao os termos utilizados são **classificado** e **não classificado** para indicar que o conscrito foi bem ou mal sucedido no processo seletivo.
 
 ### Exemplo
Para o candidato ser considerado **indicado** na fase de entrevista, os parâmetros inseridos no sistema foram os seguinte:
 - Na aba **DADOS PESSOAIS**

 Campo/parâmetro   | Indicado      | Contraindicado | 
-------------------|---------------|----------------|
 Voluntário        | Sim           |                |   
 Estado civil      | Solteiro      |                |      
 Religião          | <> Adventista |                |    
 
## Terminologia utilizada:
<table style="width: 100%; height: 205px; border-color: #000000;" border="1">
<tbody>
<tr>
<td style="text-align: center;"><strong>DESCRIÇÃO DA FASE/TERMINOLOGIA UTILIZADA</strong></td>
<td style="text-align: center;"><strong> BEM SUCEDIDO</strong></td>
<td style="text-align: center;"><strong>MAL SUCEDIDO</strong></td>
<td style="text-align: center;"><strong>COMENTÁRIO</strong></td>
</tr>
<tr>
<td>ENTREVISTA</td>
<td style="text-align: center;">Indicado</td>
<td style="text-align: center;">Contraindicado</td>
<td style="text-align: center;">&nbsp;-</td>
</tr>
<tr>
<td>AVALIAÇÃO MÉDICA</td>
<td style="text-align: center;">Apto</td>
<td style="text-align: center;">Inapto</td>
<td style="text-align: center;">&nbsp;-</td>
</tr>
<tr>
<td>AVALIAÇÃO ODONTO</td>
<td style="text-align: center;">Apto</td>
<td style="text-align: center;">Inapto</td>
<td style="text-align: center;">&nbsp;-</td>
</tr>
<tr>
<td>TESTE DE HABILIDADES</td>
<td style="text-align: center;">Demonstrou</td>
<td style="text-align: center;">Não demonstrou</td>
<td style="text-align: center;">&nbsp;-</td>
</tr>
<tr>
<td>INCORPORAÇÃO CONSCRITO</td>
<td style="text-align: center;">Classificado</td>
<td style="text-align: center;">Não classificado</td>
<td style="text-align: center;">&nbsp;-</td>
</tr>
</tbody>
</table>


<table style="width: 100%; height: 222px; border-color: #000000;" border="1">
<tbody>
<tr>
<td style="text-align: center;"><strong>CAMPO</strong></td>
<td style="text-align: center;"><strong> PARÂMETRO</strong></td>
<td style="text-align: center;"><strong>STATUS DO CONSCRITO</strong></td>
<td style="text-align: center;"><strong>ABA</strong></td>
<td style="text-align: center;"><strong>OBS</strong></td>
</tr>
<tr>
<td>ESTADO CIVIL&nbsp;</td>
<td style="text-align: center;">Solteiro</td>
<td style="text-align: center;">&nbsp;Indicado</td>
<td style="text-align: center;">DADOS PESSOAIS</td>
<td style="text-align: center;">Obrigatoriamente solteiro.</td>
</tr>
<tr>
<td>RELIGIÃO</td>
<td style="text-align: center;">&lt;&gt; Adventista</td>
<td style="text-align: center;">&nbsp;Indicado</td>
<td style="text-align: center;">DADOS PESSOAIS</td>
<td style="text-align: center;">Não pode ser adventista</td>
</tr>
<tr>
<td>ESCOLARIDADE</td>
<td style="text-align: center;">Ensino fundamental completo</td>
<td style="text-align: center;">&nbsp;Indicado</td>
<td style="text-align: center;">DADOS PESSOAIS</td>
<td style="text-align: center;">Conscrito com no mínimo o ensino fundamental completo.</td>
</tr>
<tr>
<td>VOLUNTÁRIO</td>
<td style="text-align: center;">Sim</td>
<td style="text-align: center;">&nbsp;Indicado</td>
<td style="text-align: center;">DADOS PESSOAIS</td>
<td style="text-align: center;">&nbsp;-</td>
</tr>
<tr>
<td>MORA COM QUEM NO ENDEREÇO DECLARADO</td>
<td style="text-align: center;">Pais</td>
<td style="text-align: center;">&nbsp;Indicado</td>
<td style="text-align: center;">PERFIL SOCIOECONÔMICO</td>
<td style="text-align: center;">A convivência com a família pressupõe certos atributos morais e éticos&nbsp;necessários à vida na caserna.</td>
</tr>
<tr>
<td>EM CASO DE CONVOCAÇÃO</td>
<td style="text-align: center;">&lt;&gt; Adotarei o aquartelamento como residência</td>
<td style="text-align: center;">&nbsp;Indicado</td>
<td style="text-align: center;">PERFIL SOCIOECONÔMICO</td>
<td style="text-align: center;">Laranjeira pressupõe despesas adicionais com as concessionárias, uso das instalações, outras demandas logísticas e de aprovisionamento</td>
</tr>
<tr>
<td>ARRIMO DE FAMÍLIA</td>
<td style="text-align: center;">Não</td>
<td style="text-align: center;">&nbsp;Indicado</td>
<td style="text-align: center;">PERFIL SOCIOECONÔMICO</td>
<td style="text-align: center;">O conscrito a ser incorporado não pode essencialmente ser arrimo de família .</td>
</tr>
<tr>
<td>PASSAGEM PELA POLÍCIA</td>
<td style="text-align: center;">Não</td>
<td style="text-align: center;">Indicado</td>
<td style="text-align: center;">PERFIL SOCIOECONÔMICO</td>
<td style="text-align: center;">O conscrito para ser indicado na fase de entrevista e estar em condições de concorrer á classificação não pode ter passagem pela polícia.</td>
</tr>
<tr>
<td>EXPERIÊNCIA COM DROGAS</td>
<td style="text-align: center;">Não</td>
<td style="text-align: center;">Indicado</td>
<td style="text-align: center;">PERFIL SOCIOECONÔMICO</td>
<td style="text-align: center;">O conscrito necessariamente não pode ter tido ao longo da vida experiência com drogas.</td>
</tr>
<tr>
<td>USO DE ARMA DE FOGO</td>
<td style="text-align: center;">Não</td>
<td style="text-align: center;">Indicado</td>
<td style="text-align: center;">PERFIL SOCIOECONÔMICO</td>
<td style="text-align: center;">-</td>
</tr>
</tbody>
</table>
<div></div>
<div>Unicos candidatos liberados em definitivo serão os não voluntários após passarem pela entrevista (entrevista apenas) no percentual de no máximo 50% do número de candidatos/dia.&nbsp;</div>
<div>Não há a situação de candidato sendo liberado sem passar pelo entrevistador.</div>
<div>&nbsp;</div>
<table style="width: 100%; height: 109px; border-color: #000000;" border="1">
<tbody>
<tr>
<td style="text-align: center;"><strong>DIA</strong></td>
<td style="text-align: center;"><strong> 20/01</strong></td>
<td style="text-align: center;"><strong>21/01</strong></td>
<td style="text-align: center;"><strong>22/01</strong></td>
<td style="text-align: center;"><strong>23/01</strong></td>
<td style="text-align: center;"><strong>24/01</strong></td>
<td style="text-align: center;"><strong>TOTAL</strong></td>
</tr>
<tr>
<td>QTDE/DIA</td>
<td style="text-align: center;">120</td>
<td style="text-align: center;">120</td>
<td style="text-align: center;">120</td>
<td style="text-align: center;">120</td>
<td style="text-align: center;">120</td>
<td style="text-align: center;">600</td>
</tr>
<tr>
<td>50% DE NÃO VOLUNTÁRIOS/DIA&nbsp; AINDA GARANTE A CS?</td>
<td style="text-align: center;">60</td>
<td style="text-align: center;">60</td>
<td style="text-align: center;">60</td>
<td style="text-align: center;">60</td>
<td style="text-align: center;">60</td>
<td style="text-align: center;">300</td>
</tr>
</tbody>
</table>


<table style="width: 100%; align: center; height: 205px; border-color: #000000;" border="1">
<tbody>
<tr>
<td style="text-align: center;"><strong>DESCRIÇÃO DA FASE/TERMINOLOGIA UTILIZADA</strong></td>
<td style="text-align: center;"><strong> BEM SUCEDIDO</strong></td>
<td style="text-align: center;"><strong>MAL SUCEDIDO</strong></td>
<td style="text-align: center;"><strong>COMENTÁRIO</strong></td>
</tr>
<tr>
<td>ENTREVISTA</td>
<td style="text-align: center;">Indicado</td>
<td style="text-align: center;">Contraindicado</td>
<td style="text-align: center;">&nbsp;-</td>
</tr>
<tr>
<td>AVALIAÇÃO MÉDICA</td>
<td style="text-align: center;">Apto</td>
<td style="text-align: center;">Inapto</td>
<td style="text-align: center;">&nbsp;-</td>
</tr>
<tr>
<td>AVALIAÇÃO ODONTO</td>
<td style="text-align: center;">Apto</td>
<td style="text-align: center;">Inapto</td>
<td style="text-align: center;">&nbsp;-</td>
</tr>
<tr>
<td>TESTE DE HABILIDADES</td>
<td style="text-align: center;">Demonstrou</td>
<td style="text-align: center;">Não demonstrou</td>
<td style="text-align: center;">&nbsp;-</td>
</tr>
<tr>
<td>INCORPORAÇÃO CONSCRITO</td>
<td style="text-align: center;">Classificado</td>
<td style="text-align: center;">Não classificado</td>
<td style="text-align: center;">&nbsp;-</td>
</tr>
</tbody>
</table>

