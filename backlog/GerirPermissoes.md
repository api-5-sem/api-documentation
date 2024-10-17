# Requisitos (F/NF)

## Requisitos Funcionais

- **RF-6**
- **RF-7**

## Requisitos Não Funcionais

- **RNF-3**
- **RNF-4**
- **RNF-5**

# Descrição

## Critérios de Aceite

- As permissões devem ser modulares de modo que cada funcionalidade do sistema tenha uma permissão diferente.
- As permissões incluem:
  - Visualizar lista de indicadores chaves cadastrados.
  - Criar indicador chave.
  - Deletar indicador chave.
  - Dashboard.
  - Visualizar Permissões.
  - Editar Permissões.
  - Exportar PDF.
  - Exportar EXCEL.
- Deve ser possível alterar as permissões de um usuário.
- Usuários só devem ver as funcionalidades pertinentes às suas permissões.
- Deve ser possível atribuir todas as permissões de uma só vez.
- Deve ser possível alterar mais de uma permissão de uma vez.

## Wireframe

[Abrir Wireframe](AD_4nXc8PkncB4pDD9si6RMpED3xgsDvm4BCYSKV1DhVtmc3ELJALD97uGJhOqR78E14cqbuoDAxl0QnBUmvaIEFpyHhZBSGuiczi9JTJrqAlEa7qw4G1sMaIbd54MJHwqoPtQJ5lTmWoiBu-G113Ezc7q3s3rA?key=exQ0sWSC8fbfknT6Z7lF8Q)

# BDD

---

**Dado** que um usuário tenha permissão de visualização  
**Quando** ele acessar a tela de visualizações de permissões  
**Então** ele deve visualizar todas as permissões do sistema atribuídas a um determinado usuário.

---

**Dado** que um usuário tenha permissão de edição  
**Quando** ele entrar na tela de edição de permissões  
**Então** ele deve ver todas as permissões de um determinado usuário.

---

**Dado** que um usuário tenha permissão de edição  
**Quando** ele editar uma permissão e clicar em salvar  
**Então** as permissões devem ser salvas  
**E** no próximo login deste usuário afetado, as novas permissões devem entrar em vigência.

---

**Dado** que um usuário acesse o sistema  
**Quando** ele não possuir determinada permissão  
**Então** a funcionalidade não deve aparecer para ele.
