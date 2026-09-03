---
api_key_in:
- header
api_specs:
- filename: americorps-catalog-api-openapi.yml
  format: yaml
  label: AmeriCorps Catalog API
  slug: americorps-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/americorps/refs/heads/main/openapi/americorps-catalog-api-openapi.yml
- filename: americorps-datasets-api-openapi.yml
  format: yaml
  label: AmeriCorps Datasets API
  slug: americorps-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/americorps/refs/heads/main/openapi/americorps-datasets-api-openapi.yml
- filename: americorps-metadata-api-openapi.yml
  format: yaml
  label: AmeriCorps Metadata API
  slug: americorps-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/americorps/refs/heads/main/openapi/americorps-metadata-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Americorps Authentication
name_suffix: Authentication
oauth_flows: []
overview: AmeriCorps secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AmeriCorps
provider_slug: americorps
scheme_count: 1
schemes:
- description: Optional Socrata application token. Anonymous access is allowed, but requests without a token draw from a shared per-IP pool and may be throttled.
  in: header
  legacy_alternatives:
  - in: query
    note: SODA 2.0 / 2.1 legacy form.
    parameter: $$app_token
  - in: query
    note: SODA 1.0 legacy form.
    parameter: app_token
  name: SocrataAppToken
  obtain: Register a free Socrata developer account and create an application token. No AmeriCorps approval, contract or agency relationship is involved, and there is no cost.
  parameter: X-App-Token
  required: false
  sources:
  - openapi/_original/americorps-openapi.yml
  - https://dev.socrata.com/docs/app-tokens.html
  type: apiKey
  what_it_grants: Nothing additional. Per the platform documentation a token does not confer access to any dataset an anonymous caller cannot already read — the AmeriCorps datasets are all accessLevel "public". Its only effect is that tokened requests are not throttled unless judged abusive.
slug: americorps-authentication
source_filename: americorps-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: searched\nsource: >-\n  https://dev.socrata.com/docs/app-tokens.html — the application-token reference the\n  AmeriCorps portal's API documentation link resolves to — reconciled with the\n  securitySchemes declared in openapi/_original/americorps-openapi.yml and verified by live\n  anonymous calls to data.americorps.gov on 2026-09-02.\ndocs: https://dev.socrata.com/docs/app-tokens.html\nsummary:\n  types:\n    - apiKey\n  api_key_in:\n    - header\n  anonymous_allowed: true\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  posture: >-\n    Optional-credential public API. Anonymous access is the DEFAULT and returns full data;\n    the credential is a throttling identity, not an authorization grant. Verified live:\n    GET https://data.americorps.gov/resource/fzpw-9z8s.json?$limit=1 returned 200 with data\n    and no credential presented.\nschemes:\n  - name: SocrataAppToken\n    type: apiKey\n    in: header\n    parameter: X-App-Token\n\
  \    required: false\n    description: >-\n      Optional Socrata application token. Anonymous access is allowed, but requests without a\n      token draw from a shared per-IP pool and may be throttled.\n    what_it_grants: >-\n      Nothing additional. Per the platform documentation a token does not confer access to\n      any dataset an anonymous caller cannot already read — the AmeriCorps datasets are all\n      accessLevel \"public\". Its only effect is that tokened requests are not throttled unless\n      judged abusive.\n    obtain: >-\n      Register a free Socrata developer account and create an application token. No AmeriCorps\n      approval, contract or agency relationship is involved, and there is no cost.\n    legacy_alternatives:\n      - parameter: $$app_token\n        in: query\n        note: SODA 2.0 / 2.1 legacy form.\n      - parameter: app_token\n        in: query\n        note: SODA 1.0 legacy form.\n    sources:\n      - openapi/_original/americorps-openapi.yml\n\
  \      - https://dev.socrata.com/docs/app-tokens.html\ndiscovery:\n  well_known_openid_configuration:\n    url: https://data.americorps.gov/.well-known/openid-configuration\n    status: 404\n  well_known_oauth_authorization_server:\n    url: https://data.americorps.gov/.well-known/oauth-authorization-server\n    status: 404\n  well_known_oauth_protected_resource:\n    url: https://data.americorps.gov/.well-known/oauth-protected-resource\n    status: 404\n  detail: >-\n    No authentication discovery document is served on either AmeriCorps host. An agent cannot\n    learn the auth model from the wire; it must read the docs or the OpenAPI.\nnon_public_surface:\n  note: >-\n    Private/unpublished Socrata assets return 403 rather than 404, but AmeriCorps exposes no\n    self-serve path to request access to one. The published contactPoint for the catalog is\n    Evaluation@americorps.gov (AmeriCorps Office of Research and Evaluation, from\n    https://data.americorps.gov/data.json).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/americorps/refs/heads/main/authentication/americorps-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Federal-Government
- National Service
- Volunteerism
- Community Development
- Civic Engagement
- Education
- Disaster Response
- Environmental Conservation
---
