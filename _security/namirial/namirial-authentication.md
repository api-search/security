---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: namirial-auth-api-openapi.yml
  format: yaml
  label: Namirial Auth API
  slug: namirial-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namirial/openapi/namirial-auth-api-openapi.yml
- filename: namirial-authorization-api-openapi.yml
  format: yaml
  label: Namirial Authorization API
  slug: namirial-authorization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namirial/openapi/namirial-authorization-api-openapi.yml
- filename: namirial-automaticprofile-api-openapi.yml
  format: yaml
  label: Namirial Automatic Profile API
  slug: namirial-automaticprofile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namirial/openapi/namirial-automaticprofile-api-openapi.yml
- filename: namirial-clients-api-openapi.yml
  format: yaml
  label: Namirial Clients API
  slug: namirial-clients-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namirial/openapi/namirial-clients-api-openapi.yml
- filename: namirial-clientsinstances-api-openapi.yml
  format: yaml
  label: Namirial Clients Instances API
  slug: namirial-clientsinstances-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namirial/openapi/namirial-clientsinstances-api-openapi.yml
- filename: namirial-documents-api-openapi.yml
  format: yaml
  label: Namirial Documents API
  slug: namirial-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namirial/openapi/namirial-documents-api-openapi.yml
- filename: namirial-draft-api-openapi.yml
  format: yaml
  label: Namirial Draft API
  slug: namirial-draft-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namirial/openapi/namirial-draft-api-openapi.yml
- filename: namirial-draftactivity-api-openapi.yml
  format: yaml
  label: Namirial Draft Activity API
  slug: namirial-draftactivity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namirial/openapi/namirial-draftactivity-api-openapi.yml
- filename: namirial-envelope-api-openapi.yml
  format: yaml
  label: Namirial Envelope API
  slug: namirial-envelope-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namirial/openapi/namirial-envelope-api-openapi.yml
- filename: namirial-envelopeactivity-api-openapi.yml
  format: yaml
  label: Namirial Envelope Activity API
  slug: namirial-envelopeactivity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namirial/openapi/namirial-envelopeactivity-api-openapi.yml
- filename: namirial-envelopebulk-api-openapi.yml
  format: yaml
  label: Namirial Envelope Bulk API
  slug: namirial-envelopebulk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namirial/openapi/namirial-envelopebulk-api-openapi.yml
- filename: namirial-envelopes-api-openapi.yml
  format: yaml
  label: Namirial Envelopes API
  slug: namirial-envelopes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namirial/openapi/namirial-envelopes-api-openapi.yml
- filename: namirial-file-api-openapi.yml
  format: yaml
  label: Namirial File API
  slug: namirial-file-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namirial/openapi/namirial-file-api-openapi.yml
- filename: namirial-instances-api-openapi.yml
  format: yaml
  label: Namirial Instances API
  slug: namirial-instances-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namirial/openapi/namirial-instances-api-openapi.yml
- filename: namirial-license-api-openapi.yml
  format: yaml
  label: Namirial License API
  slug: namirial-license-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namirial/openapi/namirial-license-api-openapi.yml
- filename: namirial-organizations-api-openapi.yml
  format: yaml
  label: Namirial Organizations API
  slug: namirial-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namirial/openapi/namirial-organizations-api-openapi.yml
- filename: namirial-organizationsinstances-api-openapi.yml
  format: yaml
  label: Namirial Organizations Instances API
  slug: namirial-organizationsinstances-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namirial/openapi/namirial-organizationsinstances-api-openapi.yml
- filename: namirial-processes-api-openapi.yml
  format: yaml
  label: Namirial Processes API
  slug: namirial-processes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namirial/openapi/namirial-processes-api-openapi.yml
- filename: namirial-sealingcertificate-api-openapi.yml
  format: yaml
  label: Namirial Sealing Certificate API
  slug: namirial-sealingcertificate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namirial/openapi/namirial-sealingcertificate-api-openapi.yml
- filename: namirial-system-api-openapi.yml
  format: yaml
  label: Namirial System API
  slug: namirial-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namirial/openapi/namirial-system-api-openapi.yml
- filename: namirial-team-api-openapi.yml
  format: yaml
  label: Namirial Team API
  slug: namirial-team-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namirial/openapi/namirial-team-api-openapi.yml
- filename: namirial-template-api-openapi.yml
  format: yaml
  label: Namirial Template API
  slug: namirial-template-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/namirial/openapi/namirial-template-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: derived
name: Namirial Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Namirial secures its APIs with apiKey, http, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Namirial
provider_slug: namirial
scheme_count: 4
schemes:
- description: This API uses OAuth 2 with the authorization code grant flow.
  flows:
  - authorizationUrl: /auth/authorize
    flow: authorizationCode
    scopes: 5
    tokenUrl: /auth/token
  name: oAuth2AuthCode
  sources:
  - openapi/namirial-connectors-openapi.yml
  type: oauth2
- description: This API uses OAuth 2 with the client credentials grant flow.
  flows:
  - flow: clientCredentials
    scopes: 5
    tokenUrl: /auth/token
  name: oAuth2ClientCredentials
  sources:
  - openapi/namirial-connectors-openapi.yml
  type: oauth2
- name: basicAuth
  scheme: basic
  sources:
  - openapi/namirial-connectors-openapi.yml
  type: http
- description: API Key Authentication
  in: header
  name: apiToken
  parameter: apiToken
  sources:
  - openapi/namirial-esignanywhere-openapi.yml
  type: apiKey
slug: namirial-authentication
source_filename: namirial-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: derived\nsource: openapi/namirial-connectors-openapi.yml, openapi/namirial-esignanywhere-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: oAuth2AuthCode\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /auth/authorize\n    tokenUrl: /auth/token\n    scopes: 5\n  description: This API uses OAuth 2 with the authorization code grant flow.\n  sources:\n  - openapi/namirial-connectors-openapi.yml\n- name: oAuth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /auth/token\n    scopes: 5\n  description: This API uses OAuth 2 with the client credentials grant flow.\n  sources:\n  - openapi/namirial-connectors-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/namirial-connectors-openapi.yml\n- name: apiToken\n  type: apiKey\n\
  \  in: header\n  parameter: apiToken\n  description: API Key Authentication\n  sources:\n  - openapi/namirial-esignanywhere-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/namirial/authentication/namirial-authentication.yml
summary_line: apiKey/http/oauth2 · 4 schemes
tags:
- Company
- Digital Trust
- Electronic Signature
- Identity Verification
- Digital Identity
- Trust Services
- Compliance
---
