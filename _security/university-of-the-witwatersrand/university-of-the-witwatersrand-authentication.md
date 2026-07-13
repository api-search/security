---
api_key_in: []
api_specs:
- filename: university-of-the-witwatersrand-wiredspace-rest.yaml
  format: yaml
  label: WIReDSpace DSpace REST API
  slug: wiredspace-rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-the-witwatersrand/refs/heads/main/openapi/university-of-the-witwatersrand-wiredspace-rest.yaml
- filename: university-of-the-witwatersrand-wiredspace-oai.yaml
  format: yaml
  label: WIReDSpace OAI-PMH
  slug: wiredspace-oai
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-the-witwatersrand/refs/heads/main/openapi/university-of-the-witwatersrand-wiredspace-oai.yaml
- filename: university-of-the-witwatersrand-open-data-vault.yaml
  format: yaml
  label: Wits Open Data Vault (Figshare)
  slug: open-data-vault
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-the-witwatersrand/refs/heads/main/openapi/university-of-the-witwatersrand-open-data-vault.yaml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: University Of The Witwatersrand Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: University of the Witwatersrand secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: University of the Witwatersrand
provider_slug: university-of-the-witwatersrand
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://figshare.com/account/applications/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://api.figshare.com/v2/token
  name: OAuth2
  sources:
  - openapi/university-of-the-witwatersrand-open-data-vault.yaml
  type: oauth2
slug: university-of-the-witwatersrand-authentication
source_filename: university-of-the-witwatersrand-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/university-of-the-witwatersrand-open-data-vault.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://figshare.com/account/applications/authorize\n    tokenUrl: https://api.figshare.com/v2/token\n    scopes: 1\n  sources:\n  - openapi/university-of-the-witwatersrand-open-data-vault.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-the-witwatersrand/refs/heads/main/authentication/university-of-the-witwatersrand-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Education
- Higher Education
- University
- Research
- Open Data
- Library
- Institutional Repository
- South Africa
- Africa
---
