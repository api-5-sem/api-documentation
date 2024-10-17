# Requisitos (F/NF)

## Funcionais

- **RF-1**
- **RF-2**
- **RF-3**
- **RF-7**

## Não Funcionais

- **RNF-2**
- **RNF-3**
- **RNF-4**

# Descrição

## Critérios de Aceite

Deve ser possível visualizar dashboards relacionados a:

1. **Recrutamento e seleção**:
   - Vagas em aberto (um card numérico)
   - Entrevistas marcadas para esta semana (um card numérico)
   - Número de feedbacks (um card numérico)

Cada gráfico deve ter uma descrição clara de seu propósito.  
Os dados devem ser filtrados de maneira dinâmica.  
A tela deve ser responsiva para dispositivos móveis e desktops.

## Wireframe

![Wireframe](AD_4nXcVzI87avKWESGnM1o39pTWPXG3Bzghtv2s7abYXaRAeDTUl06xxKaXjxUkmOsEsc_WNopI22m2TPxSgeYRhg4ByMsqmQov1Sv6kYKaik2Z8m3Ja2JC2NnjsEhVlccjV4_C7eK5T4pp0o2HFEp8CtplLXcI_key=exQ0sWSC8fbfknT6Z7lF8Q.png)

# BDD

---

**Dado** que eu tenha acesso ao sistema  
**Quando** eu entrar na tela inicial em resolução desktop  
**Então** eu visualizo na primeira linha da tela (1,2,3) o card de vagas em aberto, de entrevistas marcadas essa semana e de tempo médio de contratação.

---

**Dado** que eu tenha acesso ao sistema  
**Quando** eu entrar na tela inicial em resolução mobile  
**Então** eu visualizo na primeira linha da tela (6) o card de vagas em aberto, de entrevistas marcadas essa semana e de tempo médio de contratação.
