---
anonymous_access: false
api_key_in: []
api_specs:
- filename: idrive-reseller-api-openapi.yml
  format: yaml
  label: IDrive Reseller API
  slug: idrive-reseller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/idrive/refs/heads/main/openapi/idrive-reseller-api-openapi.yml
- filename: idrive-subusers-api-openapi.yml
  format: yaml
  label: IDrive Subusers API
  slug: idrive-subusers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/idrive/refs/heads/main/openapi/idrive-subusers-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Idrive Authentication
name_suffix: Authentication
oauth_flows: []
overview: IDrive declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: IDrive
provider_slug: idrive
scheme_count: 3
schemes:
- applies_to: IDrive e2 Reseller API
  description: API key generated from the profile section of the IDrive e2 account, sent in the token header on every call.
  header: token
  in: header
  name: token
  type: apiKey
- applies_to: IDrive e2 MCP (hosted)
  dynamic_client_registration: https://api.idrivee2.com/oauth/register
  evidence: https://api.idrivee2.com/oauth/.well-known/oauth-authorization-server
  flows:
  - authorization_code
  name: IDrive e2 OAuth
  pkce: S256
  type: oauth2
- applies_to: S3-compatible storage endpoints
  description: Access keys created in the e2 console or via the Reseller API create_access_key operation.
  name: S3 access keys
  type: aws-sigv4
slug: idrive-authentication
source_filename: idrive-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: searched\nsource: https://www.idrive.com/s3-storage-e2/reseller-api\nschemes:\n- name: token\n  type: apiKey\n  in: header\n  header: token\n  applies_to: IDrive e2 Reseller API\n  description: API key generated from the profile section of the IDrive e2 account, sent in the token header on every call.\n- name: IDrive e2 OAuth\n  type: oauth2\n  applies_to: IDrive e2 MCP (hosted)\n  flows:\n  - authorization_code\n  pkce: S256\n  dynamic_client_registration: https://api.idrivee2.com/oauth/register\n  evidence: https://api.idrivee2.com/oauth/.well-known/oauth-authorization-server\n- name: S3 access keys\n  type: aws-sigv4\n  applies_to: S3-compatible storage endpoints\n  description: Access keys created in the e2 console or via the Reseller API create_access_key operation.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/idrive/refs/heads/main/authentication/idrive-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Object Storage
- S3 Compatible
- Cloud Storage
- Backup
- Reseller
- MCP
---
