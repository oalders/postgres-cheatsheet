# Postgres Cheatsheet

<!-- vim-markdown-toc GFM -->

* [List All Databases](#list-all-databases)
    * [With additional columns](#with-additional-columns)
* [Connect to Database](#connect-to-database)
    * [Show Connection Info](#show-connection-info)
* [List All Functions](#list-all-functions)
* [List One Function](#list-one-function)
* [Read and/or Edit Function Definition](#read-andor-edit-function-definition)
* [List All Relations](#list-all-relations)
* [List One Relation](#list-one-relation)
* [List All Tables](#list-all-tables)
* [List All Tables Matching a Pattern](#list-all-tables-matching-a-pattern)
* [List All Tables, Views and Sequences](#list-all-tables-views-and-sequences)
* [List One Table](#list-one-table)
* [Display Privileges](#display-privileges)
* [Quit](#quit)

<!-- vim-markdown-toc -->

## List All Databases

* `\l`
* `\list`

### With additional columns

* `\l+`
* `\list+`

## Connect to Database

* `\c database_name`
* `\connect database_name`

### Show Connection Info

* `\conninfo`

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

## List One Table

* `\dt public.my_table_name`
* `\dt my_table_name`

## Display Privileges

* `\z my_relation_name`

## Quit

* `\q`
* `\quit`
