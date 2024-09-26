<h1 align="center"> Dashboard Interativo para Análise de Dados de Recrutamento e Seleção </h1>

## :books: Sobre o projeto

O projeto consiste no desenvolvimento de um dashboard interativo para centralizar e visualizar dados de recrutamento, oferecendo métricas como número de candidatos, tempo de contratação e custos. A ferramenta deve gerar relatórios dinâmicos e permitir personalizações, auxiliando a gestão na otimização do processo seletivo e na tomada de decisões estratégicas.

## :books: Solução

Criar um sistema que permita ao usuário escolher qual gráfico deverá aparecer na tela e com quais campos os dados deverão ser filtrados, de acordo com sua própria necessidade, através de uma tela de configuração interativa;
 
Criar um sistema de permissionamento modular que permite ao administrador escolher o que cada usuário pode visualizar dentro dos dashboards e do próprio sistema;

Criar um envio de notificação por email para o administrador quando determinado indicador for ultrapassado, utilizando como base o mesmo dinamismo de escolha da criação do dashboard;

Criar um sistema de exportação dos gráficos e dados vistos em tela.

<details>  
<summary><b> Requisitos do projeto: </b></summary>

## :wrench: Requisitos funcionais

     RF-1: O usuário pode escolher qual tipo de gráfico será exibido;

     RF-2: O usuário pode realizar a personalização de relatórios com filtros;

     RF-3: Cada usuário deve ter seu próprio dashboard configurável;

     RF-4: Deve ser possível a extração de qualquer relatório gerado para PDF;

     RF-5: Deve ser possível a extação de qualquer relatório gerado para Excel;

     RF-6: Deve-se criar um nível de permissionamento para todas as ações do sistema;

     RF-7: Deve-se permitir que o administrador gerencie permissões;

     RF-8: O envio de notificações por e-mail deve ocorrer sempre que os indicadores chaves ultrapassarem limites pré-definidos;

     RF-9: Os administradores podem configurar alertas automáticos com base em indicadores chave de desempenho.
     
     RF-10 Deve ser possível importar dados através de um modelo padrão
     
##  :bookmark_tabs: Requisitos não funcionais

    RNF-1: O sistema deve realizar autorização através de token JWT;

    RNF-2: O sistema deve ser compatível com os principais navegadores (Chrome, Firefox, Edge, Safari) e dispositivos móveis;

    RNF-3: O sistema deve ser intuitivo e fácil de usar;

    RNF-4: Deve ser responsivo, adaptando-se a diferentes dispositivos, como desktops, tablets e smartphones;

    RNF-5: Controle de permissões detalhado, garantindo que usuários só possam visualizar ou modificar dashboards e relatórios de acordo com seu nível de acesso;

    RNF-6: Implementar mecanismos de rollback para evitar perda de dados em caso de falhas.

</details>



## :clipboard: Backlog
<details>  
<summary> Confira o backlog do produto: </summary>
<br>
<table>
  <tr>
    <th>Rank</th>
    <th>Prioridade</th>
    <th>Feature</th>
    <th>User Story</th>
    <th>Sprint</th>
  </tr>
  <tr>
    <td>1</td>
    <td>Alta</td>
    <td>Visualizar dashboards</td>
    <td>Eu como usuário, quero poder visualizar um dashboard para que eu possa ter ciência sobre as métricas atuais de recrutamento e seleção da empresa</td>
    <td>1</td>
  </tr>
  <tr>
    <td>2</td>
    <td>Média</td>
    <td>Importar dados provisionados</td>
    <td>Eu como desenvolvedor, quero importar os dados provisionados pelo cliente para que os dados possam ser centralizados em um único banco de dados</td>
    <td>1</td>
  </tr>
  <tr>
    <td>3</td>
    <td>Alta</td>
    <td>Gerir Dashboards</td>
    <td>Eu como desenvolvedor, quero importar os dados provisionados pelo cliente para que os dados possam ser centralizados em um único banco de dados</td>
    <td>2</td>
  </tr>
  <tr>
    <td>4</td>
    <td>Alta</td>
    <td>Seleção de Indicadores personalizada</td>
    <td>Eu como administrador do sistema, quero poder criar notificações de email personalizadas com base em indicadores para que eu possa ter um direcionamento mais assertivo dos problemas da empresa</td>
    <td>2</td>
  </tr>
  <tr>
    <td>5</td>
    <td>Alta</td>
    <td>Seleção de Indicadores: envio de email</td>
    <td>Eu como administrador do sistema, quero poder receber notificações em meu email para que eu possa ser avisado quando determinado indicador for ultrapassado</td>
    <td>2</td>
  </tr>
  <tr>
    <td>6</td>
    <td>Média</td>
    <td>Autenticação de usuário</td>
    <td>Eu como usuário, quero poder realizar login na aplicação para que eu possa visualizar os dashboards do sistema</td>
    <td>2</td>
  </tr>
  <tr>
    <td>7</td>
    <td>Média</td>
    <td>Gerir permissões</td>
    <td>Eu como administrador do sistema, quero poder dar e remover permissões do usuário para que eu possa ter o controle granular de cada usuário</td>
    <td>2</td>
  </tr>
  <tr>
    <td>8</td>
    <td>Baixa</td>
    <td>Gerar Relatórios - PDF</td>
    <td>Eu como usuário, quero poder exportar um determinado dashboard para PDF para que eu tê-lo disponível offline</td>
    <td>2</td>
  </tr>
  <tr>
    <td>9</td>
    <td>Baixa</td>
    <td>Gerar Relatórios - Excel</td>
    <td>Eu como usuário, quero poder exportar um determinado dashboard para EXCEL para que eu tê-lo disponível offline</td>
    <td>2</td>
  </tr>
</table>
</details>

## :calendar: Entregas

| Sprint | Periodo | Status |
| :---: | :---: | :---: |
| 1 | 09/09/24 - 29/09/24 |  |
| 2 | 30/09/24 - 20/10/24 |  |
| 3 | 21/10/24 - 10/11/24 |  |
| 4 | 11/11/24 - 01/12/24 |  |


## :busts_in_silhouette: Equipe de desenvolvimento

| Função | Nome |
| :---: | :---: |
| Product Owner | [Matheus Cruz Fiebig](https://github.com/matheus-fiebig) |
| Scrum Master | [Wagner de Deus da Silva Júnior](https://github.com/wdeus) |
| Dev | [Alisson dos Santos Pereira](https://github.com/41issonm) |
| Dev | [Beatrice Lopes Correa](https://github.com/beatricelopes) |
| Dev | [Danillo Wesley da Costa Silva](https://github.com/xxzidanilloxx) |
| Dev | [Luciano do Nascimento Pamplona da Silva](https://github.com/lucianonps) |
