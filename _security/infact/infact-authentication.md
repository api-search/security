---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Infact Authentication
name_suffix: Authentication
oauth_flows: []
overview: InFact declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: InFact
provider_slug: infact
scheme_count: 2
schemes:
- confidential_client: true
  credentials: client_id + client_secret, issued by InFact to the customer organisation
  flow: clientCredentials
  issuer: https://connect.govconext.nl
  issuer_note: GovConext is the Netherlands government/education identity federation operated by SURF. HPZone does not run its own token endpoint in this deployment; the resource server and the authorization server are operated by different organisations.
  issuer_type: external_federation
  name: oauth2_client_credentials
  scopes:
  - standard
  - extended
  token_endpoint: https://connect.govconext.nl/oidc/token
  type: oauth2
- description: 'Non-standard: the requested data scope is ALSO sent as a plain `scope:` request header on every GraphQL POST alongside the bearer token, per the published client. An integrator that sets only the OAuth scope will not necessarily get the extended field set.'
  header_name: scope
  in: header
  name: scope_header
  type: apiKey
slug: infact-authentication
source_filename: infact-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: searched\nsource: https://cran.r-project.org/package=HPZoneAPI (HPZoneAPI 1.3.0, MIT, published 2026-04-09) — R/HPZone_setup.R\n  and R/HPZone_request.R; the package documents client_id and client_secret as \"as supplied by InFact\".\napi: HPZone API (GraphQL)\nprovider: InFact\nsummary: HPZone authenticates machine clients with OAuth 2.0 client-credentials against an EXTERNAL identity\n  provider — the Dutch government identity federation GovConext — and then carries the granted data scope\n  on every request in a custom `scope` header. InFact issues the client_id/client_secret to the customer\n  organisation; the token is minted by GovConext, not by InFact.\nschemes:\n- name: oauth2_client_credentials\n  type: oauth2\n  flow: clientCredentials\n  token_endpoint: https://connect.govconext.nl/oidc/token\n  issuer: https://connect.govconext.nl\n  issuer_type: external_federation\n  issuer_note: GovConext is the Netherlands government/education\
  \ identity federation operated by SURF.\n    HPZone does not run its own token endpoint in this deployment; the resource server and the authorization\n    server are operated by different organisations.\n  credentials: client_id + client_secret, issued by InFact to the customer organisation\n  scopes:\n  - standard\n  - extended\n  confidential_client: true\n- name: scope_header\n  type: apiKey\n  in: header\n  header_name: scope\n  description: 'Non-standard: the requested data scope is ALSO sent as a plain `scope:` request header\n    on every GraphQL POST alongside the bearer token, per the published client. An integrator that sets\n    only the OAuth scope will not necessarily get the extended field set.'\ntransport:\n  scheme: https\n  port: 8899\n  note: The data endpoint is served on a non-standard TLS port (8899), which commonly fails through corporate\n    egress filtering — our own probe could not complete a TCP connection to it (see conventions/infact-conventions.yml).\noidc_discovery:\n\
  \  url: https://connect.govconext.nl/.well-known/openid-configuration\n  status: 200\n  probed: '2026-09-02'\n  note: The GovConext discovery document is public and resolves; InFact publishes no discovery document\n    of its own.\ndocs: null\ndocs_note: InFact publishes no public authentication reference. The CRAN package description states plainly\n  that \"the API and its details are not publicly available\"; the provider-side documentation is customer-only.\nonboarding: Credentials are issued by InFact to the customer organisation; there is no self-service signup,\n  sandbox or public key issuance.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/infact/refs/heads/main/authentication/infact-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Health
- Public Health
- Healthcare
- Epidemiology
- Disease Surveillance
- Outbreak Management
- Contact Tracing
- Electronic Health Records
- openEHR
- GraphQL
- Government
---
