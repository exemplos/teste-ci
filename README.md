# teste-ci

## Configurações

.m2/settings.xml

<settings xmlns="http://maven.apache.org/SETTINGS/1.0.0"
  xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
  xsi:schemaLocation="http://maven.apache.org/SETTINGS/1.0.0
                      http://maven.apache.org/xsd/settings-1.0.0.xsd">

  <mirrors>
    <mirror>
      <id>meuNexus</id>
      <name>meuNexus</name>
      <url>http://localhost:8081/nexus/content/groups/public/</url>
      <mirrorOf>central</mirrorOf>
    </mirror>
  </mirrors>

  <servers>
     <server>
       <id>releases</id>
       <username>deployment</username>
       <password>123456</password>
     </server>
     <server>
       <id>snapshots</id>
       <username>deployment</username>
       <password>123456</password>
     </server>
  </servers>
</settings>
