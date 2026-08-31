---
api_key_in:
- header
- query
api_specs:
- filename: ferc-data-api-openapi.yml
  format: yaml
  label: FERC Data API
  slug: ferc-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ferc/refs/heads/main/openapi/ferc-data-api-openapi.yml
- filename: ferc-data-assets-api-openapi.yml
  format: yaml
  label: FERC Data Assets API
  slug: ferc-data-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ferc/refs/heads/main/openapi/ferc-data-assets-api-openapi.yml
- filename: ferc-details-api-openapi.yml
  format: yaml
  label: FERC Details API
  slug: ferc-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ferc/refs/heads/main/openapi/ferc-details-api-openapi.yml
- filename: ferc-dictionary-api-openapi.yml
  format: yaml
  label: FERC Dictionary API
  slug: ferc-dictionary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ferc/refs/heads/main/openapi/ferc-dictionary-api-openapi.yml
- filename: ferc-filing-api-openapi.yml
  format: yaml
  label: FERC Filing API
  slug: ferc-filing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ferc/refs/heads/main/openapi/ferc-filing-api-openapi.yml
- filename: ferc-public-filings-api-openapi.yml
  format: yaml
  label: FERC Public Filings API
  slug: ferc-public-filings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ferc/refs/heads/main/openapi/ferc-public-filings-api-openapi.yml
- filename: ferc-reference-api-openapi.yml
  format: yaml
  label: FERC Reference API
  slug: ferc-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ferc/refs/heads/main/openapi/ferc-reference-api-openapi.yml
- filename: ferc-taxonomy-api-openapi.yml
  format: yaml
  label: FERC Taxonomy API
  slug: ferc-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ferc/refs/heads/main/openapi/ferc-taxonomy-api-openapi.yml
auth_types:
- apiKey
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Ferc Authentication
name_suffix: Authentication
oauth_flows:
- password
overview: FERC secures its APIs with apiKey, oauth2, and http across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password flow(s).
provider_name: FERC
provider_slug: ferc
scheme_count: 4
schemes:
- api: ferc:ferc-open-data-api
  description: Recommended method per FERC's API Key Usage page — keeps the key out of the URL and out of logs. NOT declared in FERC's published OpenAPI, which only describes the query parameter; added here from the documentation.
  in: header
  name: ApiKeyHeaderAuth
  parameter: X-Api-Key
  recommended: true
  sources:
  - https://data.ferc.gov/developer/gettingstarted/api-key-usage/
  type: apiKey
- api: ferc:ferc-open-data-api
  description: Alternative method. FERC documents it as "useful for quick testing but less secure as the key becomes visible in URLs and logs."
  in: query
  name: ApiKeyQueryAuth
  parameter: api_key
  recommended: false
  sources:
  - openapi/ferc-data-api-openapi.json
  - https://data.ferc.gov/developer/gettingstarted/api-key-usage/
  type: apiKey
- api: ferc:ferc-eforms-xbrl-submission-api
  description: OAuth 2.0 Resource Owner Password Credentials grant (RFC 6749 section 4.3). Credentials are the filer's FERC eRegistration username (email) and password; the filer must be registered to file for the company. No scopes are issued.
  flow: password
  grant_parameters:
    grant_type: password
    role: filer
  name: FilerPasswordGrant
  scopes: []
  sources:
  - collections/ferc-xbrl-submission-api.postman_collection.json
  - https://www.ferc.gov/media/ferc-submission-api-step-step-guide
  tokenUrl: https://ecollection.ferc.gov/api/token
  type: oauth2
- api: ferc:ferc-eforms-xbrl-submission-api
  description: Bearer token returned by the password grant, presented on the filing endpoints.
  name: filerBearer
  scheme: bearer
  sources:
  - openapi/ferc-eforms-api-openapi-derived.yml
  type: http
slug: ferc-authentication
source_filename: ferc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: openapi/ferc-data-api-openapi.json\ndocs: https://data.ferc.gov/developer/gettingstarted/api-key-usage/\nsummary:\n  types:\n    - apiKey\n    - oauth2\n    - http\n  api_key_in:\n    - header\n    - query\n  oauth2_flows:\n    - password\n  note: >-\n    Two independent auth models. The public Open Data API uses a free 40-character API key issued by\n    email from a self-serve sign-up form; the eForms XBRL API uses an OAuth 2.0 password grant that\n    exchanges FERC eRegistration / Company Registration credentials for a bearer token. Neither API\n    issues scopes. Note that a subset of the eForms API answers with NO authentication at all — see\n    openapi/ferc-eforms-api-openapi-derived.yml.\nschemes:\n  - name: ApiKeyHeaderAuth\n    api: ferc:ferc-open-data-api\n    type: apiKey\n    in: header\n    parameter: X-Api-Key\n    recommended: true\n    description: >-\n      Recommended method per FERC's API Key Usage page\
  \ — keeps the key out of the URL and out of\n      logs. NOT declared in FERC's published OpenAPI, which only describes the query parameter; added\n      here from the documentation.\n    sources:\n      - https://data.ferc.gov/developer/gettingstarted/api-key-usage/\n  - name: ApiKeyQueryAuth\n    api: ferc:ferc-open-data-api\n    type: apiKey\n    in: query\n    parameter: api_key\n    recommended: false\n    description: >-\n      Alternative method. FERC documents it as \"useful for quick testing but less secure as the key\n      becomes visible in URLs and logs.\"\n    sources:\n      - openapi/ferc-data-api-openapi.json\n      - https://data.ferc.gov/developer/gettingstarted/api-key-usage/\n  - name: FilerPasswordGrant\n    api: ferc:ferc-eforms-xbrl-submission-api\n    type: oauth2\n    flow: password\n    tokenUrl: https://ecollection.ferc.gov/api/token\n    grant_parameters:\n      grant_type: password\n      role: filer\n    scopes: []\n    description: >-\n      OAuth 2.0 Resource\
  \ Owner Password Credentials grant (RFC 6749 section 4.3). Credentials are the\n      filer's FERC eRegistration username (email) and password; the filer must be registered to file\n      for the company. No scopes are issued.\n    sources:\n      - collections/ferc-xbrl-submission-api.postman_collection.json\n      - https://www.ferc.gov/media/ferc-submission-api-step-step-guide\n  - name: filerBearer\n    api: ferc:ferc-eforms-xbrl-submission-api\n    type: http\n    scheme: bearer\n    description: Bearer token returned by the password grant, presented on the filing endpoints.\n    sources:\n      - openapi/ferc-eforms-api-openapi-derived.yml\ncredential_issuance:\n  - api: ferc:ferc-open-data-api\n    method: self-serve web form\n    url: https://data.ferc.gov/developer/gettingstarted/sign-up-form/\n    cost: free\n    key_format: 40-character key delivered by email\n    delivery: >-\n      Usually instant; FERC documents delivery may take up to 24 hours. Lost keys are replaced by\n\
  \      re-submitting the sign-up form; old keys are deactivated on request via support.\n  - api: ferc:ferc-eforms-xbrl-submission-api\n    method: FERC eRegistration + Company Registration\n    url: https://www.ferc.gov/company-registration\n    cost: free\n    note: >-\n      Not a developer credential. The filer must be an individual registered with FERC and authorized\n      to file for a specific company CID.\nanonymous_access:\n  - api: ferc:ferc-eforms-xbrl-submission-api\n    note: >-\n      Verified 2026-07-27 — GET /PublicSubmissionHistory, /SubmissionDetail/{filingID},\n      /SubmissionHistory/forms, /getTestStatus, /TaxonomyHistory (and its file/sample/release-notes\n      children) and /faq all return HTTP 200 with no credential of any kind. FERC does not document\n      these as a public API.\nevidence:\n  - probe: GET https://api.data.ferc.gov/v1/data-assets/ with no key\n    date: '2026-07-27'\n    status: 403\n    body: '{\"error\":{\"code\":\"API_KEY_MISSING\"}}'\n \
  \ - probe: GET https://api.data.ferc.gov/v1/data-assets/?api_key=<invalid>\n    date: '2026-07-27'\n    status: 403\n    body: '{\"error\":{\"code\":\"API_KEY_INVALID\"}}'\n  - probe: GET https://ecollection.ferc.gov/api/token\n    date: '2026-07-27'\n    status: 400\n    body: '{\"error\":\"unsupported_grant_type\"}'\n  - probe: GET https://ecollection.ferc.gov/api/claims\n    date: '2026-07-27'\n    status: 401\n    body: '{\"message\":\"Authorization has been denied for this request.\"}'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ferc/refs/heads/main/authentication/ferc-authentication.yml
summary_line: apiKey/oauth2/http · 4 schemes
tags:
- Energy
- United States
- Energy Markets
- Electricity
- Natural Gas
- Grid
- Regulator
- Government
- Open Data
- Wholesale Power Markets
- Hydropower
- Oil Pipelines
---
