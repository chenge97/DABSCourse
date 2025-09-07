# Cheat Sheet for DABs commands

All commands strat with databricks bundle

deploy -t <environment> 
Deploy your bundles

validate
Validate DAB yamls

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
