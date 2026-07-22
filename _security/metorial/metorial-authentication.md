---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Metorial Authentication
name_suffix: Authentication
oauth_flows: []
overview: Metorial secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Metorial
provider_slug: metorial
scheme_count: 2
schemes:
- description: Secret API key granting full access to a project/instance. Must never be exposed in client-side code. Generated in the dashboard under Developer -> API Keys.
  format: Bearer metorial_sk_...
  header: Authorization
  in: header
  name: SecretApiKey
  prefix: metorial_sk_
  type: apiKey
- description: Publishable key for public/client-side data access. Safe to embed in client-side code; limited scope.
  format: Bearer metorial_pk_...
  header: Authorization
  in: header
  name: PublishableApiKey
  prefix: metorial_pk_
  type: apiKey
slug: metorial-authentication
source_filename: metorial-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "# Metorial authentication profile\ngenerated: '2026-07-20'\nmethod: searched\nsource: https://metorial.com/docs/api-getting-started\ndocs: https://metorial.com/docs/api-getting-started\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  scheme: bearer\nschemes:\n  - name: SecretApiKey\n    type: apiKey\n    in: header\n    header: Authorization\n    format: \"Bearer metorial_sk_...\"\n    prefix: metorial_sk_\n    description: >-\n      Secret API key granting full access to a project/instance. Must never be\n      exposed in client-side code. Generated in the dashboard under Developer -> API Keys.\n  - name: PublishableApiKey\n    type: apiKey\n    in: header\n    header: Authorization\n    format: \"Bearer metorial_pk_...\"\n    prefix: metorial_pk_\n    description: >-\n      Publishable key for public/client-side data access. Safe to embed in\n      client-side code; limited scope.\nnotes:\n  - API keys are scoped to a single instance (development or production).\n\
  \  - Metorial also brokers OAuth on behalf of downstream providers (Provider Setup Sessions), but Metorial's own API is authenticated with these bearer API keys.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metorial/refs/heads/main/authentication/metorial-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- MCP
- Model Context Protocol
- AI Agents
- Agentic Infrastructure
- Integrations
- Developer Tools
- Serverless
- API
---
