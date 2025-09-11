# Cheat Sheet for DABs commands

All commands strat with databricks bundle

deploy -t <environment> 
Deploy your bundles

validate
Validate DAB yamls
-o Output of result. Exmaple -o json
-t <environment> 
--var="nombre_de_la_var=valor para sobrescribir"

summary
Summary of our bundle

-- help 
To check available parameters

open <name of our job>
Automatically open job in UI

destroy WARNING!!!
Destroy existing bundle

run <name of our job>
Runs the job

## Where to check schema or parameters available
There is a databricks-asset-bundles.json which is a schema with all the possible paramneters available in DAB

Also, for example if you want to create a job. You can "create it" (Do all neccessary changes in UI) and before creating it you can click switch to yaml code and you can us ethat same YAML as the source of DAB code

## Variables
String variables and Complex Variables

String variables
- String

Complex
- A YAML like variable like example
clusters:
    key1: value1
    key2: value2

Retrieval variables
Variabbles that retrieve things already existing in Databricks
Example

existing_cluser:
    description: "Existing cluster"
    lookup:
        cluster: "name of existing cluster"
