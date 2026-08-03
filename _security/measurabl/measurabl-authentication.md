---
api_key_in: []
api_specs:
- filename: measurabl-core-openapi.yml
  format: yaml
  label: Measurabl Core API
  slug: measurabl-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/measurabl/refs/heads/main/openapi/measurabl-core-openapi.yml
- filename: measurabl-esgx-buildings-openapi.yml
  format: yaml
  label: Measurabl ESGx Buildings API
  slug: measurabl-esgx-buildings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/measurabl/refs/heads/main/openapi/measurabl-esgx-buildings-openapi.yml
- filename: measurabl-esgx-securities-openapi.yml
  format: yaml
  label: Measurabl ESGx Securities API
  slug: measurabl-esgx-securities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/measurabl/refs/heads/main/openapi/measurabl-esgx-securities-openapi.yml
- filename: measurabl-esgx-securities-compliance-files-openapi.yml
  format: yaml
  label: Measurabl ESGx Securities Compliance Files API
  slug: measurabl-esgx-securities-compliance-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/measurabl/refs/heads/main/openapi/measurabl-esgx-securities-compliance-files-openapi.yml
- filename: measurabl-partners-openapi.yml
  format: yaml
  label: Measurabl Partner API
  slug: measurabl-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/measurabl/refs/heads/main/openapi/measurabl-partners-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Measurabl Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Measurabl secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Measurabl
provider_slug: measurabl
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.measurabl.com/token
  name: OAuth2
  sources:
  - openapi/measurabl-core-openapi.yml
  - openapi/measurabl-esgx-buildings-openapi.yml
  - openapi/measurabl-esgx-securities-compliance-files-openapi.yml
  - openapi/measurabl-esgx-securities-openapi.yml
  - openapi/measurabl-partners-openapi.yml
  type: oauth2
slug: measurabl-authentication
source_filename: measurabl-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nsource: openapi/measurabl-core-openapi.yml, openapi/measurabl-esgx-buildings-openapi.yml, openapi/measurabl-esgx-securities-compliance-files-openapi.yml,\n  openapi/measurabl-esgx-securities-openapi.yml, openapi/measurabl-partners-openapi.yml ; upgraded from https://api.measurabl.com/api-docs/\n  and https://www.measurabl.com/measurabl-api-faq/\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\n  grant: client_credentials (RFC 6749 section 4.4)\n  token_url: https://api.measurabl.com/token\n  credential: client key + secret\n  scopes_declared: 0\n  applied_to_operations: 110\n  coverage: '100% - every operation in all five specs declares security [{OAuth2: []}]'\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.measurabl.com/token\n    scopes: 0\n  sources:\n  - openapi/measurabl-core-openapi.yml\n  - openapi/measurabl-esgx-buildings-openapi.yml\n  - openapi/measurabl-esgx-securities-compliance-files-openapi.yml\n\
  \  - openapi/measurabl-esgx-securities-openapi.yml\n  - openapi/measurabl-partners-openapi.yml\ndocs: https://support.measurabl.com/hc/en-us/articles/15889532915085-How-do-I-authenticate-with-Measurabl-s-Core-API-\nprovisioning:\n  self_serve: false\n  eligibility: Premium Tier Measurabl customer, or a partner integrating on behalf of a customer\n  process: Contact a Measurabl Customer Delivery Manager, who creates the API key and secret for the organization.\n  sales_contact: sales@measurabl.com\n  source: https://www.measurabl.com/measurabl-api-faq/\nauthorization_model:\n  style: entitlement-based\n  scopes: false\n  note: The clientCredentials flow declares an EMPTY scopes map, so there is no scope-based authorization surface.\n    Access is decided per portfolio/dataset entitlement on the credential, surfacing as 403 (\"when authenticated\n    but not authorized\") rather than as a scope error. 86 operations declare a 403 response.\ndiscovery:\n  oauth_authorization_server_metadata:\
  \ absent - /.well-known/oauth-authorization-server returns 404 on every host\n  oauth_protected_resource_metadata: absent - /.well-known/oauth-protected-resource returns 404 on every host\n  openid_configuration: absent - 404 on every host\n  note: The token endpoint is only discoverable by reading the OpenAPI securityScheme.\ntoken_transport: 'Authorization: Bearer <access_token>'\nmfa_or_mtls: null\ncross_links:\n  scopes: scopes/measurabl-scopes.yml\n  conventions: conventions/measurabl-conventions.yml\n  well_known: well-known/measurabl-well-known.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/measurabl/refs/heads/main/authentication/measurabl-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- esg
- real-estate
- sustainability
- carbon-accounting
- energy-management
- building-performance
- climate-risk
- benchmarking
- compliance
- proptech
- utility-data
- capital-markets
---
