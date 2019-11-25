# Postgres Cheatsheet

## List All Databases
* `\l`
* `\list`

### With additional columns

* `\l+`
* `\list+`

## Connect to Database
* `\c database_name`
* `\connect database_name`

## List All Functions
`\df`

## List One Function
* `\df public.my_function_name`
* `\df my_function_name`

## Read and/or Edit Function Definition

* `\ef public.my_function_name`
* `\ef my_function_name`

## List All Relations
`\d`

Note that `\d` without a pattern argument (as above) is equivalent to `\dtvs`

## List One Relation
* `\d public.my_relation_name`
* `\d my_relation_name`

## List All Tables
`\dt`

## List All Tables Matching a Pattern
* `\dt starts_with*`
* `\dt *ends_with`
* `\dt *contains*`

## List All Tables, Views and Sequences
* `\dtvs`
* `\d` (See "List All Relations")

## List One Relation
* `\dt public.my_table_name`
* `\dt my_table_name`

## Quit
* `\q`
* `\quit`