### Profile

```java
System.out.print("Hello, "); 
console.log('my name is ');  
printf("%s\n", "Dyson Parra");
```
Hello, my name is Dyson Parra  
I'm from Colombia and i'm a programmer.  

- 🌱 I’m currently learning c++
- 📍  I'm from Medellín, Antioquia (Colombia)  
- 📫 How to reach me: dysontilano@gmail.com  
<!-- 
### Hi there 👋
- 🔭 I’m looking for a job
- 🤔 I’m looking for help with ...
- 👯 I’m looking to collaborate on ...
- 💬 Ask me about ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->

### Skills
- C (source code, macros, Makefile)
- C# (source code, ASP.Net)
- Java (1.8, 11, gradle, maven, Spring, Spring boot, Eureka, Hibernate, Sonatype, Selenium)
- Python (Source code, pandas, pyspark)
- Angular (Typescript, CSS, Html, javascript, Postman)
- Sql (Mariadb, Mysql, Sql server, Postgress)
- Android Studio (With java)
- Use of Regex (Perl cli, sed cli, vs code)
- Snowflake data cloud
- Databricks
- AWS (Sam cli, S3, lambda, layer, Kms)
- Azure functions
- Matillon Dev
- Redshift
- Domo
- Tableau
- Windows scripts (bat)
- Linux scripts (sh)

### Repository naming

<details>
  <summary>details</summary>
  
  The repositories are not named randomly, their names specify information about its following the patterns:
  - Language:  
    All the repositories ends with '-' and next the language (or languages) in which are written, using the primary extension of the language or the language name.

    For example:  
    * the repos could be ends with '-java', '-c', '-cs', '-cpp', '-py', '-js', '-android' (because if '-java' is used could be confused), '-angular,' etc.  
    
  - Type of repository:  
    The type of repo is specified at the start of the name of the repo and are two types, applications and projects:
      * Applications:  
        The repos that starts with 'app-' or 'lib-' are repos with apps that could be run and the difference is that if starts with 'app-' is
        simplely an application, but if starts wth 'lib-' is an app with code that is being used or could be reused in other repos as library.
        - Type of application:  
          If the repo is an app (or lib) then specify the type of app:
          * CLI (Console app):  
            If next to the type of repo is 'cli-', so the repo start name could be 'app-cli-' or 'lib-cli-'.
          * GUI (Stand alone app with a gui):  
            If next to the type of repo is 'gui-', so the repo start name could be 'app-gui-' or 'lib-gui-'.
          * MOB (Mobile application):  
            If next to the type of repo is 'mob-', so the repo start name could be 'app-mob-' or 'lib-mob-'.
          * WEB (Web application):  
            If next to the type of repo is 'web-', so the repo start name could be 'app-web-' or 'lib-web-'.
         
        For example:  
        - If the repo contains an application written in c withouth graphic interface that is used to process json files (Parsing, write the file in console, etc)
            with the app name 'json-processor', and the code could be used in another repos to parse json files (is a library) the repo name will be
            'lib-cli-json-processor-c'.
        - If the repo contains an application written in android studio with graphic interface that is used to touch piano keys and listen their sound
          with the name 'piano-keys', but the code is not usable as library in another apps or repos, the repo name will be 'app-mob-piano-keys-android'

      * Projects:  
        The repos that starts with 'proj-' are repos with various apps or apps and additional files just like postman scripts, sql scripts and other files
        that are neccesary for the app, but are not part of the code.
        - Type of project:  
        There are two types of projects, full or module:
          * Full project (All):  
            If the next word of the type of repo is '-all', so the repo starts with 'proj-all-', the repository contains varios apps or apps and info insite of them,
            and the apps inside could be there with the full code or as submodule.
          * Module project (mod):
            If the next word of the type of repo is '-mod', so the repo starts with 'proj-mod-', the repository contains an application that is part of a project,
            but the source code is independient of the project, and inside of the full project is contained as submodule.
         
        For example:  
        - If the repo contains two apps, the front and the back end of a crud written in java and angular, its sql scripts for a mysql database named
          'veterinary' and the name of the project is the same that the database, the repo name will be 'proj-all-veterinary-mysql-java-angular'
          with the next tree struct:
          
          /proj-all-veterinary-mysql-java-angular  
          ├── backend  
          │   ├── app-cli-veterinary-java  
          ├── frontend  
          │   ├── app-web-veterinary-angular  
          ├── sql  
          │   ├── mysql_database_veterinay_create.sql  
   
          Observe that at the end of the repository name the three languages used are specified, instead of if the repo were an app, and that the apps
          included inside of the repo (back and front) keep the same pattern that if they were an independient repo.

        - If the case is the same that the previos, but after considering is not convenient to has the code of frontend and backend in the same repo,
          but if they are sepparated as independient repos could be hard to known with these names that they belong to the same project, in this case
          are usefull the module naming, so at start of the the repo add the indicative that is a module of the repo (proj-mod-) next the project name
          (veterinary), keep the rest of the name and include the backend and frontend as submodules of the full project, so the result is:
          
          /proj-all-veterinary-mysql-java-angular  
          ├── backend  
          │   ├── proj-mod-veterinary-app-cli-veterinary-java (Submodule)  
          ├── frontend  
          │   ├── proj-mod-veterinary-app-web-veterinary-angular (Submodule)  
          ├── sql  
          │   ├── mysql_database_veterinay_create.sql  

  
      If this git account contains various additional repos for example all the repos are:  
      * app-gui-piano-keys-java
      * app-mob-piano-keys-android
      * lib-cli-json-processor-c
      * lib-cli-xml-processor-py
      * proj-all-pharmacy-mysql-java-angular
      * proj-all-veterinary-mysql-java-angular
      * proj-mod-veterinary-app-cli-veterinary-java
      * proj-mod-veterinary-app-web-veterinary-angular

      Is easy to identify that:  
      * There are four app (two apps and two libs).
      * The apps are written in android studio (mobile) and java (cli), and the libraries are written in c (cli) and python (cli).
      * There are four projects (two full projects and two modules of a full project).  
      * The project 'pharmaciy' has not submodules, so all the apps source code or info are inside the same repo.
      * The project 'veterinary' has a complete project and inside two submodules that are as independient repositories.
      * The projects 'pharmaciy' and 'veterinary' use mysql, java and angular.
      * One submodule of the project 'veterinary' use java (cli).
      * One submodule of the project 'veterinary' use angular (web).
      
      That is identified only with the name of the repository.
</details>

### Relevant projects

<details>
  <summary>details</summary>
  
  - Examples of connection to a database and CRUD services using spring and hibernate.  
    Create database script (mysql) and postman tests file also included.  
  [almacen](https://github.com/DysonParra/proj-almacen-back-mysql-java)  
  [appointments](https://github.com/DysonParra/proj-appointments-back-mysql-java)  
  [autopistas](https://github.com/DysonParra/proj-autopistas-back-mysql-java)  
  [farmacias](https://github.com/DysonParra/proj-farmacias-back-mysql-java)  
  [minas](https://github.com/DysonParra/proj-minas-back-mysql-java)  
  [restaurant](https://github.com/DysonParra/proj-restaurant-back-mysql-java)  
  [veterinaria](https://github.com/DysonParra/proj-veterinaria-back-mysql-java)  
  [vias](https://github.com/DysonParra/proj-vias-back-mysql-java)  
  
  - Examples of connection to a database and CRUD services using ASP.NET and entity framework.  
    Create database script (sql server) also included.  
  [Almacen](https://github.com/DysonParra/proj-almacen-back-front-sql-server-cs)  
  [Appointments](https://github.com/DysonParra/proj-appointments-back-front-sql-server-cs)  
  [Autopistas](https://github.com/DysonParra/proj-autopistas-back-front-sql-server-cs)  
  [Farmacias](https://github.com/DysonParra/proj-farmacias-back-front-sql-server-cs)  
  [Minas](https://github.com/DysonParra/proj-minas-back-front-sql-server-cs)  
  [Restaurant](https://github.com/DysonParra/proj-restaurant-back-front-sql-server-cs)  
  [Veterinaria](https://github.com/DysonParra/proj-veterinaria-back-front-sql-server-cs)  
  [Vias](https://github.com/DysonParra/proj-vias-back-front-sql-server-cs)  
    
  - Flag processors:  
  Cli lib that receive an undetermined number of arguments, analyze if are correctly formed and if yes parse it into objects (or structs) or else print the specific error in console.  
  The flags are from two types (you can use the two at same time):  
    * With value: an alphanumeric string started with '-' and the next argument must be the value of the flag.  
    Example:  -downloadPath documents   -sourceFile myFile.xml   -rootDir C:/project  
    * Withouth value: an alphanumerirc string started with '--'.  
    Example:  --useDefault  --notUseIncognito  --generateLogFile  --preserveTempFiles  

    For use the library you need to specify in source code a set of flags defined as required, other defined as optionals and other defined as default. More specific how to use in the projects.  
    [c](https://github.com/DysonParra/lib-cli-flag-processor-c)  
    [c#](https://github.com/DysonParra/lib-cli-flag-processor-cs)  
    [java](https://github.com/DysonParra/lib-cli-flag-processor-java)  
    [python](https://github.com/DysonParra/lib-cli-flag-processor-py)  
  
</details>
