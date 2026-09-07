---
anonymous_access: true
api_key_in:
- header
api_specs:
- filename: cancer-gov-seer-openapi.yml
  format: yaml
  label: NCI SEER API
  slug: seer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cancer-gov/refs/heads/main/openapi/cancer-gov-seer-openapi.yml
- filename: cancer-gov-modac-openapi.yml
  format: yaml
  label: NCI MoDaC API
  slug: modac-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cancer-gov/refs/heads/main/openapi/cancer-gov-modac-openapi.yml
- filename: cancer-gov-evs-openapi.yml
  format: yaml
  label: NCI EVS Terminology API
  slug: evs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cancer-gov/refs/heads/main/openapi/cancer-gov-evs-openapi.yml
- filename: cancer-gov-diseases-api-openapi.yml
  format: yaml
  label: Cancer.gov Diseases API
  slug: cancer-gov-diseases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cancer-gov/refs/heads/main/openapi/cancer-gov-diseases-api-openapi.yml
- filename: cancer-gov-interventions-api-openapi.yml
  format: yaml
  label: Cancer.gov Interventions API
  slug: cancer-gov-interventions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cancer-gov/refs/heads/main/openapi/cancer-gov-interventions-api-openapi.yml
- filename: cancer-gov-terms-api-openapi.yml
  format: yaml
  label: Cancer.gov Terms API
  slug: cancer-gov-terms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cancer-gov/refs/heads/main/openapi/cancer-gov-terms-api-openapi.yml
- filename: cancer-gov-trials-api-openapi.yml
  format: yaml
  label: Cancer.gov Trials API
  slug: cancer-gov-trials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cancer-gov/refs/heads/main/openapi/cancer-gov-trials-api-openapi.yml
- filename: cancer-gov-glossary-openapi.yml
  format: yaml
  label: NCI Glossary Term API
  slug: glossary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cancer-gov/refs/heads/main/openapi/cancer-gov-glossary-openapi.yml
- filename: cancer-gov-drug-dictionary-openapi.yml
  format: yaml
  label: NCI Drug Dictionary API
  slug: drug-dictionary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cancer-gov/refs/heads/main/openapi/cancer-gov-drug-dictionary-openapi.yml
- filename: cancer-gov-sitewide-search-openapi.yml
  format: yaml
  label: Cancer.gov Site-Wide Search API
  slug: sitewide-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cancer-gov/refs/heads/main/openapi/cancer-gov-sitewide-search-openapi.yml
- filename: cancer-gov-best-bets-openapi.yml
  format: yaml
  label: Cancer.gov Best Bets API
  slug: best-bets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cancer-gov/refs/heads/main/openapi/cancer-gov-best-bets-openapi.yml
- filename: cancer-gov-r4r-openapi.yml
  format: yaml
  label: NCI Resources for Researchers API
  slug: r4r-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cancer-gov/refs/heads/main/openapi/cancer-gov-r4r-openapi.yml
auth_types:
- apiKey
- none
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Cancer Gov Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cancer.gov secures its APIs with apiKey and none across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Cancer.gov
provider_slug: cancer-gov
scheme_count: 5
schemes:
- api: cancer-gov:clinical-trials-api
  description: Free API key issued by the CTS Developer Accounts portal at https://clinicaltrialsapi.cancer.gov/.
  evidence: Live GET https://clinicaltrialsapi.cancer.gov/api/v2/trials without a key returns HTTP 401 {"message":"Forbidden"}.
  in: header
  name: apiKey
  parameter: X-API-KEY
  required: true
  sources:
  - openapi/cancer-gov-trials-api-openapi.yml
  - https://www.cancer.gov/syndication/api
  type: apiKey
- api: cancer-gov:seer-api
  description: Free SEER*API account key. The terms of service govern use and state a 5,000-call/60-minute ceiling.
  evidence: components.securitySchemes.apiKeyScheme in https://api.seer.cancer.gov/v3/api-docs; live GET /rest/glossary/latest returns HTTP 401 anonymously.
  in: header
  name: apiKeyScheme
  parameter: X-SEERAPI-Key
  required: true
  sources:
  - openapi/cancer-gov-seer-openapi.yml
  - https://api.seer.cancer.gov/terms
  type: apiKey
- api: cancer-gov:gdc-api
  description: Token downloaded from the GDC Data Portal or Data Submission Portal. Needed only for controlled-access data and submission; open-access data and the GraphQL endpoint answer anonymously.
  evidence: 'Documented at https://docs.gdc.cancer.gov/API/Users_Guide/Getting_Started/. Confirmed live: GET https://api.gdc.cancer.gov/status and an anonymous POST introspection to /v0/graphql both return HTTP 200. Not derivable from a spec — the GDC publishes no OpenAPI.'
  in: header
  name: gdcAuthToken
  parameter: X-Auth-Token
  required: false
  sources:
  - https://docs.gdc.cancer.gov/API/Users_Guide/Getting_Started/
  type: apiKey
- api: cancer-gov:evs-api
  description: The EVS REST API declares no securityScheme and requires no credential.
  evidence: Live GET https://api-evsrest.nci.nih.gov/api/v1/metadata/terminologies returns HTTP 200 anonymously.
  name: none
  required: false
  sources:
  - openapi/cancer-gov-evs-openapi.yml
  type: none
- api: cancer-gov:glossary-api
  description: None of the five webapis.cancer.gov services (glossary, drugdictionary, sitewidesearch, bestbets, r4r) declares a securityScheme or requires a credential.
  evidence: No components.securitySchemes in any of the five NSwag-generated specs served under https://webapis.cancer.gov/*/v1/swagger/v1/swagger.json.
  name: none
  required: false
  sources:
  - openapi/cancer-gov-glossary-openapi.yml
  - openapi/cancer-gov-drug-dictionary-openapi.yml
  - openapi/cancer-gov-sitewide-search-openapi.yml
  - openapi/cancer-gov-best-bets-openapi.yml
  - openapi/cancer-gov-r4r-openapi.yml
  type: none
slug: cancer-gov-authentication
source_filename: cancer-gov-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: 'Derived from securitySchemes in the eight first-party OpenAPI documents, then upgraded from NCI''s\n  own documentation: https://docs.gdc.cancer.gov/API/Users_Guide/Getting_Started/ (X-Auth-Token), https://api.seer.cancer.gov/terms\n  and https://api.seer.cancer.gov/docs, and https://www.cancer.gov/syndication/api (free CTS key). Anonymous\n  access was confirmed live for EVS and the webapis.cancer.gov services.'\ndocs: https://docs.gdc.cancer.gov/API/Users_Guide/Getting_Started/\nsummary:\n  types:\n  - apiKey\n  - none\n  api_key_in:\n  - header\n  oauth2: false\n  openIdConnect: false\n  mutualTLS: false\n  note: 'Three different API-key header names across three services, and five services with no authentication\n    at all. There is no single NCI credential: a client integrating across this estate registers separately\n    with each program.'\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n\
  \  api: cancer-gov:clinical-trials-api\n  required: true\n  description: Free API key issued by the CTS Developer Accounts portal at https://clinicaltrialsapi.cancer.gov/.\n  evidence: Live GET https://clinicaltrialsapi.cancer.gov/api/v2/trials without a key returns HTTP 401\n    {\"message\":\"Forbidden\"}.\n  sources:\n  - openapi/cancer-gov-trials-api-openapi.yml\n  - https://www.cancer.gov/syndication/api\n- name: apiKeyScheme\n  type: apiKey\n  in: header\n  parameter: X-SEERAPI-Key\n  api: cancer-gov:seer-api\n  required: true\n  description: Free SEER*API account key. The terms of service govern use and state a 5,000-call/60-minute\n    ceiling.\n  evidence: components.securitySchemes.apiKeyScheme in https://api.seer.cancer.gov/v3/api-docs; live GET\n    /rest/glossary/latest returns HTTP 401 anonymously.\n  sources:\n  - openapi/cancer-gov-seer-openapi.yml\n  - https://api.seer.cancer.gov/terms\n- name: gdcAuthToken\n  type: apiKey\n  in: header\n  parameter: X-Auth-Token\n  api:\
  \ cancer-gov:gdc-api\n  required: false\n  description: Token downloaded from the GDC Data Portal or Data Submission Portal. Needed only for controlled-access\n    data and submission; open-access data and the GraphQL endpoint answer anonymously.\n  evidence: 'Documented at https://docs.gdc.cancer.gov/API/Users_Guide/Getting_Started/. Confirmed live:\n    GET https://api.gdc.cancer.gov/status and an anonymous POST introspection to /v0/graphql both return\n    HTTP 200. Not derivable from a spec — the GDC publishes no OpenAPI.'\n  sources:\n  - https://docs.gdc.cancer.gov/API/Users_Guide/Getting_Started/\n- name: none\n  type: none\n  api: cancer-gov:evs-api\n  required: false\n  description: The EVS REST API declares no securityScheme and requires no credential.\n  evidence: Live GET https://api-evsrest.nci.nih.gov/api/v1/metadata/terminologies returns HTTP 200 anonymously.\n  sources:\n  - openapi/cancer-gov-evs-openapi.yml\n- name: none\n  type: none\n  api: cancer-gov:glossary-api\n\
  \  required: false\n  description: None of the five webapis.cancer.gov services (glossary, drugdictionary, sitewidesearch,\n    bestbets, r4r) declares a securityScheme or requires a credential.\n  evidence: No components.securitySchemes in any of the five NSwag-generated specs served under https://webapis.cancer.gov/*/v1/swagger/v1/swagger.json.\n  sources:\n  - openapi/cancer-gov-glossary-openapi.yml\n  - openapi/cancer-gov-drug-dictionary-openapi.yml\n  - openapi/cancer-gov-sitewide-search-openapi.yml\n  - openapi/cancer-gov-best-bets-openapi.yml\n  - openapi/cancer-gov-r4r-openapi.yml\noauth:\n  supported: false\n  note: No oauth2 or openIdConnect scheme anywhere; no /.well-known/oauth-authorization-server or /openid-configuration\n    on any of the 11 hosts probed (all 404).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cancer-gov/refs/heads/main/authentication/cancer-gov-authentication.yml
summary_line: apiKey/none · 5 schemes
tags:
- Cancer
- Federal-Government
- Healthcare
- Research
- Clinical Trials
- Genomics
- Surveillance
- Open Data
---
