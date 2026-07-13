---
api_key_in: []
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Oracle REST Data Services (ORDS)
  slug: oracle-rest-data-services-ords
  spec_type: OpenAPI
  url: https://docs.oracle.com/en/database/oracle/oracle-rest-data-services/
- filename: openapi.yaml
  format: yaml
  label: Oracle Cloud Infrastructure Database API
  slug: oracle-cloud-infrastructure-database-api
  spec_type: OpenAPI
  url: https://docs.oracle.com/iaas/api/#/en/database/
- filename: oracle-database-soda-openapi.yml
  format: yaml
  label: Oracle SODA (Simple Oracle Document Access)
  slug: oracle-soda-simple-oracle-document-access
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-database/refs/heads/main/openapi/oracle-database-soda-openapi.yml
- filename: oracle-database-txeventq-asyncapi.yml
  format: yaml
  label: Oracle Transactional Event Queues (TxEventQ)
  slug: oracle-transactional-event-queues-txeventq
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-database/refs/heads/main/asyncapi/oracle-database-txeventq-asyncapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Oracle Database Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Oracle Database secures its APIs with http and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Oracle Database
provider_slug: oracle-database
scheme_count: 4
schemes:
- description: OCI request signature authentication using API signing keys
  name: ociSignature
  scheme: bearer
  sources:
  - openapi/oracle-database-oci-openapi.yml
  type: http
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: /ords/{schema}/oauth/token
  - authorizationUrl: /ords/{schema}/oauth/auth
    flow: authorizationCode
    scopes: 0
    tokenUrl: /ords/{schema}/oauth/token
  name: oauth2
  sources:
  - openapi/oracle-database-ords-openapi.yml
  type: oauth2
- name: basicAuth
  scheme: basic
  sources:
  - openapi/oracle-database-ords-openapi.yml
  - openapi/oracle-database-soda-openapi.yml
  type: http
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: /ords/{schema}/oauth/token
  name: oauth2
  sources:
  - openapi/oracle-database-soda-openapi.yml
  type: oauth2
slug: oracle-database-authentication
source_filename: oracle-database-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/oracle-database-oci-openapi.yml, openapi/oracle-database-ords-openapi.yml, openapi/oracle-database-soda-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: ociSignature\n  type: http\n  scheme: bearer\n  description: OCI request signature authentication using API signing keys\n  sources:\n  - openapi/oracle-database-oci-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /ords/{schema}/oauth/token\n    scopes: 0\n  - flow: authorizationCode\n    authorizationUrl: /ords/{schema}/oauth/auth\n    tokenUrl: /ords/{schema}/oauth/token\n    scopes: 0\n  sources:\n  - openapi/oracle-database-ords-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/oracle-database-ords-openapi.yml\n  - openapi/oracle-database-soda-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n\
  \  - flow: clientCredentials\n    tokenUrl: /ords/{schema}/oauth/token\n    scopes: 0\n  sources:\n  - openapi/oracle-database-soda-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oracle-database/refs/heads/main/authentication/oracle-database-authentication.yml
summary_line: http/oauth2 · 4 schemes
tags:
- Cloud
- Database
- Enterprise
- Oracle
- REST API
- SQL
---
