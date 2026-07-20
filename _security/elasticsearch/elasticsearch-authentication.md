---
api_key_in:
- header
api_specs:
- filename: elasticsearch-specification
  format: yaml
  label: Elasticsearch REST API
  slug: elasticsearch-rest-api
  spec_type: OpenAPI
  url: https://github.com/elastic/elasticsearch-specification
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Elasticsearch Authentication
name_suffix: Authentication
oauth_flows: []
overview: Elasticsearch secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Elasticsearch
provider_slug: elasticsearch
scheme_count: 2
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/elasticsearch-openapi.yml
  type: http
- docs: https://www.elastic.co/docs/reference/elasticsearch/rest-apis/create-api-keys
  format: '"Authorization: ApiKey <base64(id:api_key)>"'
  in: header
  name: apiKeyAuth
  parameter: Authorization
  sources:
  - openapi/elasticsearch-openapi.yml
  type: apiKey
slug: elasticsearch-authentication
source_filename: elasticsearch-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: openapi/elasticsearch-openapi.yml\ndocs: https://www.elastic.co/docs/deploy-manage/users-roles/cluster-or-deployment-auth\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  model: >-\n    Elasticsearch REST API authentication is per-cluster. HTTP Basic and API\n    keys are the primary programmatic mechanisms; the security layer also\n    supports bearer/service tokens, PKI (mutual TLS), and enterprise SSO realms\n    (SAML, OIDC, Kerberos, LDAP/Active Directory). Authorization is\n    role-based (RBAC) via cluster and index privileges, not OAuth scopes.\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/elasticsearch-openapi.yml\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: '\"Authorization: ApiKey <base64(id:api_key)>\"'\n  docs: https://www.elastic.co/docs/reference/elasticsearch/rest-apis/create-api-keys\n  sources:\n  - openapi/elasticsearch-openapi.yml\n\
  realms:\n- native\n- api_key\n- token (bearer / service account tokens)\n- pki (mutual TLS)\n- saml\n- oidc\n- kerberos\n- ldap\n- active_directory\nauthorization:\n  model: rbac\n  concepts:\n    - cluster privileges\n    - index privileges\n    - application privileges\n    - roles and role mappings\n  docs: https://www.elastic.co/docs/deploy-manage/users-roles/cluster-or-deployment-auth/user-roles\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elasticsearch/refs/heads/main/authentication/elasticsearch-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Analytics
- Database
- Full-Text Search
- NoSQL
- Search
---
