# Datasource generator #


## Usage: ##

### Datasource: ###
Dballocator:
`-datasourceName <name> -jndiName <name> -driverName <driver> -dballocatorProperties <path>`

Attributes:
`-databaseFamily <family> -datasourceName <name> -jndiName <name> -driverName <driver> -connectionUrl <jdbc url> -username <username> -password <password> -jta <true/false> -useJavaContext <true/false>`

### XA Datasource: ###
#### Dballocator: ####
`-xa -datasourceName <name> -jndiName <name> -driverName <driver> -dballocatorProperties <path>`

#### Attributes: ####
`-xa -datasourceName <name> -jndiName <name> -driverName <driver> -username <username> -password <password> -xaDatasourceClass <xa-datasource-class> -xaProps <name=value,name1=value1...>`

### General options: ###
`-out filename` to output the xml to a file (ds.xml)

`-config standalone.xml` output the datsource xml to standalone.xml configuration file

## Development: ##

####Gradle tasks: ####

`gradle clean`

`gradle build`

`gradle distZip`

###### run dist: ######
`./bin/eap6-ds-creator parameters`

###### run: ######
`java -cp './build/libs/eap6-ds-creator-1.1.0.Final.jar:<path-to>/groovy-all-2.2.1.jar:<path-to>/commons-cli-1.2.jar'  org.jboss.qe.dscreator.Main parameters`


