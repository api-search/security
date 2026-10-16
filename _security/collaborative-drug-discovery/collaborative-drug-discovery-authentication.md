---
anonymous_access: false
api_key_in: []
api_specs:
- filename: collaborative-drug-discovery-openapi.json
  format: json
  label: CDD Vault API
  slug: cdd-vault-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/collaborative-drug-discovery/refs/heads/main/openapi/collaborative-drug-discovery-openapi.json
auth_types: []
description: Authentication schemes as published on Collaborative Drug Discovery support pages.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Collaborative Drug Discovery Authentication
name_suffix: Authentication
oauth_flows: []
overview: Collaborative Drug Discovery declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Collaborative Drug Discovery
provider_slug: collaborative-drug-discovery
scheme_count: 1
schemes:
- evidence: Every API request must include the "X-CDD-Token" HTTP header.
  header: X-CDD-Token
  how_to_obtain: Obtain through the API Key management page by navigating to Settings → User → API Keys page after API access has been enabled for the vault.
  location: header
  name: X-CDD-Token
  type: apiKey
slug: collaborative-drug-discovery-authentication
source_filename: collaborative-drug-discovery-authentication.yml
source_heading: Authentication Profile
source_url: https://support.collaborativedrug.com/hc/en-us/articles/214358363-Second-factor-authentication-with-Duo
source_yaml: "generated: '2026-10-09'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://support.collaborativedrug.com/hc/en-us/articles/214358363-Second-factor-authentication-with-Duo\nsources:\n- https://support.collaborativedrug.com/hc/en-us/articles/214358363-Second-factor-authentication-with-Duo\n- https://support.collaborativedrug.com/hc/en-us/articles/115005682263-Token-based-Authentication\ndescription: Authentication schemes as published on Collaborative Drug Discovery support pages.\nschemes:\n- type: apiKey\n  name: X-CDD-Token\n  evidence: Every API request must include the \"X-CDD-Token\" HTTP header.\n  location: header\n  header: X-CDD-Token\n  how_to_obtain: Obtain through the API Key management page by navigating to Settings → User → API Keys page after API access has been enabled\n    for the vault.\nnote: No OAuth2 or other authentication schemes were described on the provided pages.\ndocs: https://support.collaborativedrug.com/hc/en-us/articles/214358363-Second-factor-authentication-with-Duo\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/collaborative-drug-discovery/refs/heads/main/authentication/collaborative-drug-discovery-authentication.yml
summary_line: 1 scheme
tags:
- Scientific Data Management
- Lab Informatics
- Pharmaceutical
- Academic Research
- Collaboration
---
