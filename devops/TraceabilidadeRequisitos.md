### Pré-requisitos
Para realizar o monitoramento requisitos é necessário primeiro que alguns padrões sejam seguidos, sendo eles:
   <ul>
      <li>
         <a href="https://github.com/api-5-sem/api-documentation/blob/main/devops/Versionamento_E_FluxoTrabalho.md">Versionamento e Fluxo de Trabalho.</a>  
      </li>
      <ul>
         <li>Motivo: permite controlar qual “commit” esta vinculado a qual história e a intenção daquele dele (correção, nova feature, etc)</li>
      </ul>
   </ul>   
   <ul>
      <li>Preenchimento dos requisitos da história pelo PO</li>
      <ul>
         <li>Motivo: determinar de qual requisito aquela história deu origem </li>
      </ul>
   </ul>
   <ul>
      <li>Todos requisitos funcionais/não-funcionais estão centralizados no <a href="#">documento de requisitos</a></li>
      <ul>
         <li>Motivo: facilidade de identificação dos requisitos do projeto</li>
      </ul>
   </ul>
   <ul>
      <li>DoD/DOR esta sendo realizado em toda as histórias</li>
      <ul>
         <li>Motivo: demarcação dos projetos/requisitos que estão sendo afetados em uma determinada história</li>
      </ul>
   </ul>

### Relação Requisito X História
Para encontrar a relação descrita acima basta entrar no link que se encontra logo abaixo de cada tópico na pagina de <a href="#">Proposta de Solução e Requisitos</a>  

OBS: é possível realizar consultas mais complexas utilizando JQL caso necessário
Ex: "Requisitos(F/NF)[Paragraph]" ~ "RF-3" OR "Requisitos(F/NF)[Paragraph]" ~ "RF-4"
 
### Funcionamento

### Observação
Devido ao DoD e possível, também, descobrir se uma determinada historia impactou ou não determinado sistema. Para isso basta atentar-se ao campo de Sistemas Afetados, localizado logo abaixo do DoD nas historias.
