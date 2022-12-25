Sistema de Acompanhamento da Seleção Complementar 👋

### 1 - INTRODUÇÃO AO SisASC
Seja bem vindo ao **Sistema de Acompanhamento da Seleção Complementar - SisASC/16º BI Mtz**. O SisASC é um instrumento de gestão e controle e foi concebido para ser a ferramenta de coleta de dados dos conscritos durante a execução da seleção complementar na OM.

### 2 - COMPOSIÇÃO DO SisASC
O sistema é composto basicamente de uma **Ficha de Entrevista (Digital)** e de um **Menu de opções**. 
 - Ficha Digital de Entrevista (FDE): é composta por um conjunto de abas (`DADOS PESSOAIS`, `TÍTULO DE ELEITOR`, `CNH`, `INSPEÇÃO MÉDICA`, `INSPEÇÃO ODONTOLÓGICA`, `TESTE DE HABILIDADES`, `PERFIL SOCIOECONÔMICO`, etc). Em cada aba da FDE os campos de formulário foram agrupados respeitando a afinidade que os dados guardam entre si.
 - Menu de opções: os menus agrupam, também por afinidade, as diversas consultas (relatórios) disponíveis no SisASC.

![menus e abas 1](https://user-images.githubusercontent.com/121310141/209476833-cc7f8c83-6f32-494e-a391-2d6f78e0b27c.png)

Na imagem acima temos a aba DADOS PESSOAIS em evidência. 

Repare que o sistema recusa o cadastramanto do conscrito se os campos NOME, CPF, ESTADO CIVIL, RELIGIÃO, ESCOLARIDADE, e ENTREVISTADOR não forem corretamente preenchidos. O campo CPF do formulário tem validação *isunique*, garantindo que cada CPF armazenado no banco de dados seja único. De outra forma, o sistema não permitirá a duplicidade de cadastro.  

  
### 3 - CARACTERÍSTICAS DO SisASC
No SisASC os atributos/características desejáveis no conscrito (Perfil do Candidato) são os parametros que foram configurados no sistema e que podem ser alterados a critéro do Cmt OM.

O sistema possui as configurações necessárias para garantir que todos os conscritos selecionados para a incorporação, atendam aos requisitos que a unidade deseja. Para que o conscrito seja considerado indicado na entrevista, uma série de requisitos devem ser satisfeitos; para que o conscrito seja contraindicado na fase de entrevista, todavia, basta que apenas um dos parâmetros (requisitos) não seja atendido. Essas características do sistema garantem o rigor e a homogeneidade do processo seletivo. 

No entanto se o número necessário de conscritos para o preenchimento dos `claros` não for atingido, a critério do Cmt OM, os parâmerros podem ser flexibilizados obedecendo a uma precedência definida pelo Cmt OM. 
> **Note**
> Não existe no sistema o botão `Indicado`, ou `indicar candidato`, ou `ndicar conscrito`. Essa tarefa foi automatizada, significando dizer que o próprio sistema se encarregará de indicar (ou contraindicar) o conscrito a partir dos dados coletados na FDE em confronto com os parâmetros configurados.

> **Warning**
> A situação de contraindicado durante a fase de entrevista, depende da negação de apenas um dos parâmetros.

**Exemplo**: no campo RELIGIÃO da aba DADOS PESSOAIS, se o valor selecionado for "Adventista", o conscrito será automaticamente contraindicado independente de quais sejam as respostas para os demais campos utilizados como parâmetros.

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

### 4 - TERMINOLOGIA UTILIZADA NO SisASC
 DESCRIÇÃO DA FASE/TERMO UTILIZADO | BEM SUCEDIDO |   MAL SUCEDIDO   | 
-----------------------------------|--------------|------------------|
 Entrevista                        | Indicado     | Contraindicado   |   
 Inspeção médica                   | Apto         | Inapto           |      
 Inspeção odonto                   | Apto         | Inapto           |      
 Teste habilidades                 | Demonstrou   | Não demonstrou   |      
 Incorporação                      | Classificado | Não clasiificado |      
 
> **Note** 
> Na fase de entrevista o sistema adota os termos **indicado** e **contraindicado** para significar que o conscrito foi bem ou mal sucedido durante essa etapa do processo; na fase de inspeção médica e odontológica os termos utilizados são **apto** e **inapto** para inddicar que o conscrito foi bem ou mal sucedido nessa fase da seleção de pessoal; na fase onde são verificadas as habilidades declaradas pelo conscrito, os termos utilizados são **demonstrou** e **não demonstrou** a competência declarada; na última etapa da seleçãao os termos utilizados são **classificado** e **não classificado** para indicar que o conscrito foi bem ou mal sucedido no processo seletivo.

## 5 - PARÂMETROS DE CONFIGURAÇÃO UTILIZADOS NO SisASC:
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
    
## 6 - CONCEPÇÃO DE UMA SC UTILIZANDO O SisASC:
>**Note**
>Unicos candidatos liberados em definitivo serão os não voluntários após passarem pela entrevista (entrevista apenas) no percentual de no máximo 50% do número de candidatos/dia.&nbsp; 

>**Warning**
> Não há a hipóteses de o candidato sendo liberado sem passar pelo entrevistador.
 
 
 






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


 ### Exemplo
Para o candidato ser considerado **indicado** na fase de entrevista, os parâmetros inseridos no sistema foram os seguinte:
 - Na aba **DADOS PESSOAIS**

 Campo/parâmetro   | Indicado      | Contraindicado | 
-------------------|---------------|----------------|
 Voluntário  ✔️   | Sim           |                |   
 Estado civil      | Solteiro      |                |      
 Religião          | <> Adventista |                |   
 
 <details>
<summary>:eyes: Show example</summary>

<picture>
<source 
  srcset="https://github-readme-stats.vercel.app/api?username=anuraghazra&show_icons=true&theme=dark"
  media="(prefers-color-scheme: dark)"
/>
<source
  srcset="https://github-readme-stats.vercel.app/api?username=anuraghazra&show_icons=true"
  media="(prefers-color-scheme: light), (prefers-color-scheme: no-preference)"
/>
<img src="https://github-readme-stats.vercel.app/api?username=anuraghazra&show_icons=true" />
</picture>

</details>
 
 
