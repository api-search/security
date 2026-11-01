---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Light And Wonder Authentication
name_suffix: Authentication
oauth_flows: []
overview: Light & Wonder declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Light & Wonder
provider_slug: light-and-wonder
scheme_count: 1
schemes:
- additional_parameters:
  - description: client id parameter of the service call
    name: client-id
  - description: property id of the Light & Wonder
    name: property-id
  evidence: 'Access Token URI:[ex:http://{Rest API Based Service URL}/oauth?grant_type=client_credentials] Client id: Username of the token service Client Secret: password of the token service'
  flow: clientCredentials
  name: oauth2-client-credentials
  provisioning: Credentials and the per-property service URL are requested from the Light & Wonder point of contact; the host is deployment-specific ({hostname}:{port}), not a public multi-tenant endpoint.
  token_url_pattern: http://{Rest API Based Service URL}/oauth?grant_type=client_credentials
  type: oauth2
slug: light-and-wonder-authentication
source_filename: light-and-wonder-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: searched\nsource: https://docs.oracle.com/en/industries/hospitality/enterprise-integrations/gaming-integration/25.1/gamig/c_light_wonder_cmp_acsc.htm\ndocs: https://docs.oracle.com/en/industries/hospitality/enterprise-integrations/gaming-integration/25.1/gamig/c_light_wonder_cmp_acsc.htm\nscope: Light & Wonder CMP (casino management) webservices, as documented by a THIRD PARTY (Oracle Hospitality OPERA Cloud gaming integration guide). Light & Wonder publishes no public API documentation of its own; its Gateway integration docs (gateway.lnw.com) sit behind an Okta/Auth0 customer login.\nschemes:\n- name: oauth2-client-credentials\n  type: oauth2\n  flow: clientCredentials\n  token_url_pattern: http://{Rest API Based Service URL}/oauth?grant_type=client_credentials\n  evidence: 'Access Token URI:[ex:http://{Rest API Based Service URL}/oauth?grant_type=client_credentials] Client id: Username of the token service Client Secret: password of the token\
  \ service'\n  additional_parameters:\n  - name: client-id\n    description: client id parameter of the service call\n  - name: property-id\n    description: property id of the Light & Wonder\n  provisioning: Credentials and the per-property service URL are requested from the Light & Wonder point of contact; the host is deployment-specific ({hostname}:{port}), not a public multi-tenant endpoint.\nnote: Third-party evidence only. The scheme describes the on-property CMP webservices consumed by OPERA Cloud, not a publicly callable Light & Wonder API.\n"
source_yaml_url: https://artifacts.apis.io/light-and-wonder/authentication/light-and-wonder-authentication.yml
summary_line: 1 scheme
tags:
- Gaming
- Casinos
- iGaming
- Mobile Games
- Entertainment
- Slot Machines
- Social Gaming
---
