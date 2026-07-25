---
api_key_in:
- header
auth_types:
- apiKey
- none
description: ''
kind: authentication
layout: security
method: searched
name: Fca Uk Authentication
name_suffix: Authentication
oauth_flows: []
overview: Financial Conduct Authority secures its APIs with apiKey and none across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Financial Conduct Authority
provider_slug: fca-uk
scheme_count: 2
schemes:
- api: FCA Financial Services Register API
  base_url: https://register.fca.org.uk/services/V0.1
  cost: free
  evidence:
  - body: '{"Success":"false", "Sorry, this page is not available. Missing Headers."}'
    kind: live probe
    note: The API rejects the anonymous request for missing auth headers rather than 404ing the route.
    request: GET https://register.fca.org.uk/services/V0.1/Firm/122702
    status: 403
  - kind: third-party client documentation
    note: 'Community Python client shows the prepared request headers {''Accept'': ''application/json'', ''X-Auth-Email'': ..., ''X-Auth-Key'': ...}. The FCA''s own reference documentation for these headers sits behind the portal login and is not anonymously verifiable.'
    url: https://financial-services-register-api.readthedocs.io/en/latest/sources/usage.html
  in: header
  name: FSRegisterHeaderAuth
  obtained_via: Free self-serve registration at https://register.fca.org.uk/Developer/s/ (a Salesforce Experience Cloud login wall with a "Register to be a New User" path). The key is generated from the registration profile.
  parameters:
  - description: The email address the developer registered with on the FS Register developer portal.
    name: X-Auth-Email
  - description: The API key generated from the developer portal profile.
    name: X-Auth-Key
  type: apiKey
- api: FCA Data Publication API (FIRDS / FITRS file query)
  base_url: https://api.data.fca.org.uk
  description: The documented machine-to-machine file-listing interface behind data.fca.org.uk requires no credentials. Only the two documented indices respond anonymously.
  evidence:
  - kind: live probe
    request: GET https://api.data.fca.org.uk/fca_data_firds_files?q=*&size=1
    status: 200
  - kind: live probe
    request: GET https://api.data.fca.org.uk/fca_data_fitrs_files?q=*&size=1
    status: 200
  - body: Missing Authentication Token
    kind: live probe
    note: Undocumented sibling index names all return 403; only the two indices the FCA documents in its published technical specifications are public.
    request: GET https://api.data.fca.org.uk/fca_data_ssr_current?q=*&size=1
    status: 403
  name: DataPublicationAnonymous
  type: none
slug: fca-uk-authentication
source_filename: fca-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: >-\n  https://www.fca.org.uk/firms/financial-services-register ; live anonymous probes\n  of https://register.fca.org.uk/services/V0.1/* and https://api.data.fca.org.uk/* ;\n  https://register.fca.org.uk/.well-known/openid-configuration ;\n  https://www.fca.org.uk/publication/systems-information/fca-firds-tech-spec.pdf\nnote: >-\n  The FCA publishes no OpenAPI, so this profile is assembled from the FCA's own\n  public pages and technical specifications plus live anonymous probes, not\n  derived from securitySchemes. Two different auth models operate on two\n  different FCA API surfaces, and a third (OIDC) belongs to the portal only.\nsummary:\n  types: [apiKey, none]\n  api_key_in: [header]\n  oauth2_flows: []\n  openapi_derived: false\nschemes:\n- name: FSRegisterHeaderAuth\n  type: apiKey\n  in: header\n  api: FCA Financial Services Register API\n  base_url: https://register.fca.org.uk/services/V0.1\n  parameters:\n  - name:\
  \ X-Auth-Email\n    description: The email address the developer registered with on the FS Register developer portal.\n  - name: X-Auth-Key\n    description: The API key generated from the developer portal profile.\n  obtained_via: >-\n    Free self-serve registration at https://register.fca.org.uk/Developer/s/ (a\n    Salesforce Experience Cloud login wall with a \"Register to be a New User\"\n    path). The key is generated from the registration profile.\n  cost: free\n  evidence:\n  - kind: live probe\n    request: GET https://register.fca.org.uk/services/V0.1/Firm/122702\n    status: 403\n    body: '{\"Success\":\"false\", \"Sorry, this page is not available. Missing Headers.\"}'\n    note: The API rejects the anonymous request for missing auth headers rather than 404ing the route.\n  - kind: third-party client documentation\n    url: https://financial-services-register-api.readthedocs.io/en/latest/sources/usage.html\n    note: >-\n      Community Python client shows the prepared request\
  \ headers\n      {'Accept': 'application/json', 'X-Auth-Email': ..., 'X-Auth-Key': ...}.\n      The FCA's own reference documentation for these headers sits behind the\n      portal login and is not anonymously verifiable.\n- name: DataPublicationAnonymous\n  type: none\n  api: FCA Data Publication API (FIRDS / FITRS file query)\n  base_url: https://api.data.fca.org.uk\n  description: >-\n    The documented machine-to-machine file-listing interface behind\n    data.fca.org.uk requires no credentials. Only the two documented indices\n    respond anonymously.\n  evidence:\n  - kind: live probe\n    request: GET https://api.data.fca.org.uk/fca_data_firds_files?q=*&size=1\n    status: 200\n  - kind: live probe\n    request: GET https://api.data.fca.org.uk/fca_data_fitrs_files?q=*&size=1\n    status: 200\n  - kind: live probe\n    request: GET https://api.data.fca.org.uk/fca_data_ssr_current?q=*&size=1\n    status: 403\n    body: Missing Authentication Token\n    note: >-\n      Undocumented\
  \ sibling index names all return 403; only the two indices the\n      FCA documents in its published technical specifications are public.\nportal_identity:\n  protocol: openid-connect\n  scope: developer portal login only — NOT the Register API\n  discovery: https://register.fca.org.uk/.well-known/openid-configuration\n  captured: well-known/fca-uk-openid-configuration.json\n  issuer: https://register.fca.org.uk\n  authorization_endpoint: https://register.fca.org.uk/services/oauth2/authorize\n  token_endpoint: https://register.fca.org.uk/services/oauth2/token\n  note: >-\n    Served by the Salesforce Experience Cloud platform hosting the Register site.\n    The scopes_supported list is the stock Salesforce platform set (cdp_api,\n    wave_api, pardot_api, chatter_api, mcp_api, ...) and does not describe any\n    FCA API permission model, which is why no scopes/ artifact is emitted.\nnot_present:\n  mutual_tls: false\n  oauth2_for_apis: false\n  scopes: >-\n    No scope model exists on\
  \ either FCA API surface — the Register API is a flat\n    header key with full read access, the data publication API is anonymous.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fca-uk/refs/heads/main/authentication/fca-uk-authentication.yml
summary_line: apiKey/none · 2 schemes
tags:
- Insurance
- United Kingdom
- Regulator
- Market Infrastructure
- Financial Services
- Public Register
- Conduct Regulation
- Open Finance
- Insurance Intermediaries
- Risk Data
- Market Data
- Reference Data
- MiFID II
---
