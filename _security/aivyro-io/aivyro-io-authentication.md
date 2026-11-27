---
anonymous_access: false
api_key_in: []
api_specs:
- filename: aivyro-io-openapi-generated.yml
  format: yaml
  label: Aivyro API
  slug: aivyro-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aivyro-io/openapi/_ae-authored/aivyro-io-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Aivyro Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aivyro declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Aivyro
provider_slug: aivyro-io
scheme_count: 1
schemes:
- bearerFormat: aivk_
  description: Chave de API com prefixo aivk_. Não enviada via query nem cookie.
  scheme: bearer
  scopes:
  - description: Leitura de contatos
    name: rest.crm.contacts.read
  - description: Criação/atualização de contatos
    name: rest.crm.contacts.write
  - description: Leitura de empresas
    name: rest.crm.companies.read
  - description: Criação/atualização de empresas
    name: rest.crm.companies.write
  - description: Leitura de negócios
    name: rest.crm.deals.read
  - description: Criação/atualização de negócios
    name: rest.crm.deals.write
  - description: Leitura de notas
    name: rest.crm.notes.read
  - description: Criação/atualização de notas
    name: rest.crm.notes.write
  - description: Leitura de tarefas
    name: rest.crm.tasks.read
  - description: Criação/atualização de tarefas
    name: rest.crm.tasks.write
  - description: Leitura de webhooks
    name: rest.crm.webhooks.read
  - description: Criação/atualização de webhooks
    name: rest.crm.webhooks.write
  - description: Leitura de tags
    name: rest.crm.tags.read
  - description: Criação/atualização de tags
    name: rest.crm.tags.write
  - description: Leitura de reuniões
    name: rest.meetings.read
  - description: Leitura de conversas
    name: rest.conversations.read
  - description: Envio de mensagens e respostas
    name: rest.conversations.write
  - description: Leitura de sequências
    name: rest.sequences.read
  - description: Inscrição em sequências
    name: rest.sequences.write
  type: http
slug: aivyro-io-authentication
source_filename: aivyro-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: searched\nsource: https://knowledge.aivyro.io/start/authentication\nschemes:\n  - type: http\n    scheme: bearer\n    bearerFormat: aivk_\n    description: \"Chave de API com prefixo aivk_. Não enviada via query nem cookie.\"\n    scopes:\n      - name: rest.crm.contacts.read\n        description: \"Leitura de contatos\"\n      - name: rest.crm.contacts.write\n        description: \"Criação/atualização de contatos\"\n      - name: rest.crm.companies.read\n        description: \"Leitura de empresas\"\n      - name: rest.crm.companies.write\n        description: \"Criação/atualização de empresas\"\n      - name: rest.crm.deals.read\n        description: \"Leitura de negócios\"\n      - name: rest.crm.deals.write\n        description: \"Criação/atualização de negócios\"\n      - name: rest.crm.notes.read\n        description: \"Leitura de notas\"\n      - name: rest.crm.notes.write\n        description: \"Criação/atualização de notas\"\n      -\
  \ name: rest.crm.tasks.read\n        description: \"Leitura de tarefas\"\n      - name: rest.crm.tasks.write\n        description: \"Criação/atualização de tarefas\"\n      - name: rest.crm.webhooks.read\n        description: \"Leitura de webhooks\"\n      - name: rest.crm.webhooks.write\n        description: \"Criação/atualização de webhooks\"\n      - name: rest.crm.tags.read\n        description: \"Leitura de tags\"\n      - name: rest.crm.tags.write\n        description: \"Criação/atualização de tags\"\n      - name: rest.meetings.read\n        description: \"Leitura de reuniões\"\n      - name: rest.conversations.read\n        description: \"Leitura de conversas\"\n      - name: rest.conversations.write\n        description: \"Envio de mensagens e respostas\"\n      - name: rest.sequences.read\n        description: \"Leitura de sequências\"\n      - name: rest.sequences.write\n        description: \"Inscrição em sequências\"\n"
source_yaml_url: https://artifacts.apis.io/aivyro-io/authentication/aivyro-io-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Revenue Engineering
- Platform
- CRM
- Analytics
---
