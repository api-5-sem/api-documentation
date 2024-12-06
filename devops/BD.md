#  DevOps BD 

Este documento descreve o processo de configuração e execução do DevOps para um projeto de banco de dados utilizando Flyway e PostgreSQL.  

---

## **Etapa 1: Configuração**

## 📁 Estrutura do Projeto
### **1.1 Instalação**

<details open>
#### Dependências Maven
<b>Adicione as dependências abaixo no arquivo `pom.xml` </b> 

```xml
<!-- Flyway para PostgreSQL -->
<dependency>
    <groupId>org.flywaydb</groupId>
    <artifactId>flyway-database-postgresql</artifactId>
</dependency>

<dependency>
    <groupId>org.flywaydb</groupId>
    <artifactId>flyway-core</artifactId>
</dependency>
```

#### Plugin Maven
<b> Inclua o plugin Flyway no `pom.xml` para gerenciar as migrações</b> 
:
```xml
<plugin>
    <groupId>org.flywaydb</groupId>
    <artifactId>flyway-maven-plugin</artifactId>
    <version>10.21.0</version> <!-- Atualize para a versão desejada -->
    <configuration>
        <url>jdbc:postgresql://localhost:5432/dash</url>
        <user>admin</user>
        <password>admin</password>
        <schemas>public</schemas>
        <locations>
            <location>classpath:bd/migration</location>
        </locations>
    </configuration>
</plugin>
```
</details>

### **1.2 Configuração do Projeto**

<details open>
<b> Estrutura de diretórios </b> 

```plaintext
migrations/
    sprint_1/
        V1__create_table_users.sql
        V2__add_column_email.sql
    sprint_2/
        V3__create_table_orders.sql

```
<b> Configurações no application.properties </b> 

```plaintext
spring.application.name=pixel
spring.datasource.url=jdbc:postgresql://localhost:5432/dash
spring.datasource.username=admin
spring.datasource.password=admin
spring.datasource.driver-class-name=org.postgresql.Driver

spring.flyway.enabled=true
spring.flyway.locations=classpath:bd/migration

spring.jpa.open-in-view=false

```

</details>


## **Etapa 2: Execução**

## 📁 Estrutura do Projeto

### **2.1  Criar Scripts de Migração**

<details open>
<b> Exemplo: migrations/sprint_1/V1__create_table_users.sql</b> 

```sql
CREATE TABLE users (
    id SERIAL PRIMARY KEY,
    name VARCHAR(100),
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);

```
</details>


### **2.2  Criar Scripts de Rollback**
<details open>
<b> U2__drop_sprint2_table.sql</b> 

```sql
DROP TABLE IF EXISTS public.config_Indicador;
DELETE FROM flyway_schema_history WHERE version = '2';


```

</details>

### **2.3  Comandos Flyway**
<details open>
<b>Validar migrações</b> 

```plaintext
flyway validate

```
<b>Validar migrações</b> 

```plaintext
flyway migrate
mvn spring-boot:run


```

</details>

### **2.4  Teste de Carga**

<details open>

<b>Instale as dependências</b> 

```plaintext
pip install pandas faker

```
<b>Execute o script de teste</b> 

```plaintext
python testeCarga.py



```
O script testeCarga.py gera automaticamente dados de carga inicial para o banco.

</details>





