---
api_key_in:
- header
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Keboola Storage API
  slug: storage-api
  spec_type: OpenAPI
  url: https://api.keboola.com/?service=storage
- filename: openapi.yaml
  format: yaml
  label: Keboola Management API
  slug: management-api
  spec_type: OpenAPI
  url: https://api.keboola.com/?service=manage
- filename: openapi.yaml
  format: yaml
  label: Keboola Queue API
  slug: queue-api
  spec_type: OpenAPI
  url: https://api.keboola.com/?service=job-queue
- filename: openapi.yaml
  format: yaml
  label: Keboola Scheduler API
  slug: scheduler-api
  spec_type: OpenAPI
  url: https://api.keboola.com/?service=scheduler
- filename: openapi.yaml
  format: yaml
  label: Keboola Developer Portal API
  slug: developer-portal-api
  spec_type: OpenAPI
  url: https://api.keboola.com/?service=developer-portal
- filename: openapi.yaml
  format: yaml
  label: Keboola Encryption API
  slug: encryption-api
  spec_type: OpenAPI
  url: https://api.keboola.com/?service=encryption
- filename: openapi.yaml
  format: yaml
  label: Keboola Notifications API
  slug: notifications-api
  spec_type: OpenAPI
  url: https://api.keboola.com/?service=notification
- filename: openapi.yaml
  format: yaml
  label: Keboola OAuth Broker API
  slug: oauth-broker-api
  spec_type: OpenAPI
  url: https://api.keboola.com/?service=oauth
- filename: openapi.yaml
  format: yaml
  label: Keboola Stream API
  slug: stream-api
  spec_type: OpenAPI
  url: https://api.keboola.com/?service=stream
- filename: openapi.yaml
  format: yaml
  label: Keboola Query API
  slug: query-api
  spec_type: OpenAPI
  url: https://api.keboola.com/?service=query
- filename: openapi.yaml
  format: yaml
  label: Keboola Sandboxes Service API
  slug: sandboxes-api
  spec_type: OpenAPI
  url: https://api.keboola.com/?service=sandboxes-service
- filename: openapi.yaml
  format: yaml
  label: Keboola Vault API
  slug: vault-api
  spec_type: OpenAPI
  url: https://api.keboola.com/?service=vault
- filename: openapi.yaml
  format: yaml
  label: Keboola Billing API
  slug: billing-api
  spec_type: OpenAPI
  url: https://api.keboola.com/?service=billing
- filename: openapi.yaml
  format: yaml
  label: Keboola AI API
  slug: ai-api
  spec_type: OpenAPI
  url: https://api.keboola.com/?service=ai
- filename: openapi.yaml
  format: yaml
  label: Keboola Importer API
  slug: importer-api
  spec_type: OpenAPI
  url: https://api.keboola.com/?service=import
- filename: openapi.yaml
  format: yaml
  label: Keboola Editor API
  slug: editor-api
  spec_type: OpenAPI
  url: https://api.keboola.com/?service=editor
- filename: openapi.yaml
  format: yaml
  label: Keboola Synchronous Actions API
  slug: sync-actions-api
  spec_type: OpenAPI
  url: https://api.keboola.com/?service=sync-actions
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Keboola Authentication
name_suffix: Authentication
oauth_flows: []
overview: Keboola secures its APIs with apiKey and http across 6 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Keboola
provider_slug: keboola
scheme_count: 6
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-StorageApi-Token
  sources:
  - openapi/keboola-ai-api-openapi.yml
  - openapi/keboola-billing-api-openapi.yml
  - openapi/keboola-editor-api-openapi.yml
  - openapi/keboola-importer-api-openapi.yml
  - openapi/keboola-management-api-openapi.yml
  - openapi/keboola-notifications-api-openapi.yml
  - openapi/keboola-oauth-broker-api-openapi.yml
  - openapi/keboola-queue-api-openapi.yml
  - openapi/keboola-sandboxes-api-openapi.yml
  - openapi/keboola-scheduler-api-openapi.yml
  - openapi/keboola-storage-api-openapi.yml
  - openapi/keboola-stream-api-openapi.yml
  - openapi/keboola-sync-actions-api-openapi.yml
  - openapi/keboola-vault-api-openapi.yml
  type: apiKey
- description: Application token with scope "billing:manage"
  in: header
  name: BillingManageToken
  parameter: X-KBC-ManageApiToken
  sources:
  - openapi/keboola-billing-api-openapi.yml
  - openapi/keboola-encryption-api-openapi.yml
  - openapi/keboola-management-api-openapi.yml
  - openapi/keboola-oauth-broker-api-openapi.yml
  - openapi/keboola-sandboxes-api-openapi.yml
  - openapi/keboola-storage-api-openapi.yml
  type: apiKey
- description: JWT token from `POST /auth/login`, passed verbatim (no "Bearer " prefix). Admin endpoints require a token belonging to an administrator.
  in: header
  name: bearerAuth
  parameter: Authorization
  sources:
  - openapi/keboola-developer-portal-api-openapi.yml
  type: apiKey
- bearerFormat: Access Token (kbc_at_...)
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/keboola-management-api-openapi.yml
  - openapi/keboola-storage-api-openapi.yml
  type: http
- in: header
  name: ApplicationTokenAuth
  parameter: X-Kbc-ManageApiToken
  sources:
  - openapi/keboola-notifications-api-openapi.yml
  type: apiKey
- in: header
  name: StorageApiToken
  parameter: X-StorageAPI-Token
  sources:
  - openapi/keboola-query-api-openapi.yml
  type: apiKey
slug: keboola-authentication
source_filename: keboola-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/keboola-ai-api-openapi.yml, openapi/keboola-billing-api-openapi.yml, openapi/keboola-developer-portal-api-openapi.yml,\n  openapi/keboola-editor-api-openapi.yml, openapi/keboola-encryption-api-openapi.yml, openapi/keboola-importer-api-openapi.yml,\n  openapi/keboola-management-api-openapi.yml, openapi/keboola-notifications-api-openapi.yml,\n  openapi/keboola-oauth-broker-api-openapi.yml, openapi/keboola-query-api-openapi.yml, openapi/keboola-queue-api-openapi.yml,\n  openapi/keboola-sandboxes-api-openapi.yml ...\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-StorageApi-Token\n  sources:\n  - openapi/keboola-ai-api-openapi.yml\n  - openapi/keboola-billing-api-openapi.yml\n  - openapi/keboola-editor-api-openapi.yml\n  - openapi/keboola-importer-api-openapi.yml\n  - openapi/keboola-management-api-openapi.yml\n  - openapi/keboola-notifications-api-openapi.yml\n\
  \  - openapi/keboola-oauth-broker-api-openapi.yml\n  - openapi/keboola-queue-api-openapi.yml\n  - openapi/keboola-sandboxes-api-openapi.yml\n  - openapi/keboola-scheduler-api-openapi.yml\n  - openapi/keboola-storage-api-openapi.yml\n  - openapi/keboola-stream-api-openapi.yml\n  - openapi/keboola-sync-actions-api-openapi.yml\n  - openapi/keboola-vault-api-openapi.yml\n- name: BillingManageToken\n  type: apiKey\n  in: header\n  parameter: X-KBC-ManageApiToken\n  description: Application token with scope \"billing:manage\"\n  sources:\n  - openapi/keboola-billing-api-openapi.yml\n  - openapi/keboola-encryption-api-openapi.yml\n  - openapi/keboola-management-api-openapi.yml\n  - openapi/keboola-oauth-broker-api-openapi.yml\n  - openapi/keboola-sandboxes-api-openapi.yml\n  - openapi/keboola-storage-api-openapi.yml\n- name: bearerAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: JWT token from `POST /auth/login`, passed verbatim (no \"Bearer \" prefix). Admin\n \
  \   endpoints require a token belonging to an administrator.\n  sources:\n  - openapi/keboola-developer-portal-api-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: Access Token (kbc_at_...)\n  sources:\n  - openapi/keboola-management-api-openapi.yml\n  - openapi/keboola-storage-api-openapi.yml\n- name: ApplicationTokenAuth\n  type: apiKey\n  in: header\n  parameter: X-Kbc-ManageApiToken\n  sources:\n  - openapi/keboola-notifications-api-openapi.yml\n- name: StorageApiToken\n  type: apiKey\n  in: header\n  parameter: X-StorageAPI-Token\n  sources:\n  - openapi/keboola-query-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keboola/refs/heads/main/authentication/keboola-authentication.yml
summary_line: apiKey/http · 6 schemes
tags:
- Data Platform
- ETL
- ELT
- Data Pipelines
- Data Storage
- Transformations
- Orchestration
- Data Operations
- Cloud Data
- Snowflake
- BigQuery
---
