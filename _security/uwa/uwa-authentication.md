---
api_key_in:
- header
- query
api_specs:
- filename: uwa-oai-pmh-openapi.yml
  format: yaml
  label: UWA Research Repository OAI-PMH
  slug: oai-pmh
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uwa/refs/heads/main/openapi/uwa-oai-pmh-openapi.yml
auth_types:
- none
- apiKey
- saml2
description: ''
kind: authentication
layout: security
method: probed
name: Uwa Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Western Australia secures its APIs with none, apiKey, and saml2 across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: University of Western Australia
provider_slug: uwa
scheme_count: 3
schemes:
- description: The OAI-PMH endpoint at https://api.research-repository.uwa.edu.au/ws/oai is fully open. All six OAI-PMH 2.0 verbs returned 200 with no credential presented, including ListRecords over persons:all and publications:all. This is the only UWA-operated API surface reachable without an account.
  name: none
  sources:
  - https://api.research-repository.uwa.edu.au/ws/oai?verb=Identify
  surface: uwa:oai-pmh
  type: none
  x-operator: institution
- confidence: medium
  description: api-portal.uwa.edu.au is a Microsoft Azure API Management developer portal ("Discover APIs, learn how to use them, try them out interactively, and sign up to acquire keys"), and api.uwa.edu.au answers as a live APIM gateway (HTTP/2 404, content-type application/json, Azure request-context header). Azure APIM's subscription-key header is the platform default. Marked medium confidence because the product catalog is behind sign-in — the specific header name and any per-product override could not be read without an account, and /signup returns 404. No key was obtained and no protected operation was called.
  in: header
  name: azure-apim-subscription-key
  parameter: Ocp-Apim-Subscription-Key
  sources:
  - https://api-portal.uwa.edu.au/
  - https://api.uwa.edu.au/
  surface: uwa:developer-portal
  type: apiKey
  x-operator: institution
- description: UWA operates its own Shibboleth SAML 2.0 identity provider at https://idp.uwa.edu.au/idp/shibboleth, scoped to uwa.edu.au, with HTTP-POST and HTTP-Redirect SingleSignOnService bindings and transient NameID. This is the credential behind essentially every affiliation-gated UWA service, and it is the institution's most significant machine-readable, standards-based surface.
  name: shibboleth-saml2
  sources:
  - https://idp.uwa.edu.au/idp/shibboleth
  surface: uwa:identity-federation
  type: saml2
  x-operator: institution
slug: uwa-authentication
source_filename: uwa-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: >-\n  Live probes on 2026-08-30 of https://api.research-repository.uwa.edu.au/ws/oai,\n  https://api-portal.uwa.edu.au/, https://api.uwa.edu.au/ and https://idp.uwa.edu.au/idp/shibboleth.\n  Replaces a previous file whose only source was Elsevier's Pure Web Service OpenAPI — that\n  contract is the vendor's and has been removed from this repo.\nx-operator: institution\nsummary:\n  types:\n  - none\n  - apiKey\n  - saml2\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: none\n  type: none\n  surface: uwa:oai-pmh\n  x-operator: institution\n  description: >-\n    The OAI-PMH endpoint at https://api.research-repository.uwa.edu.au/ws/oai is fully open. All\n    six OAI-PMH 2.0 verbs returned 200 with no credential presented, including ListRecords over\n    persons:all and publications:all. This is the only UWA-operated API surface reachable without\n    an account.\n  sources:\n  - https://api.research-repository.uwa.edu.au/ws/oai?verb=Identify\n\
  - name: azure-apim-subscription-key\n  type: apiKey\n  in: header\n  parameter: Ocp-Apim-Subscription-Key\n  surface: uwa:developer-portal\n  x-operator: institution\n  confidence: medium\n  description: >-\n    api-portal.uwa.edu.au is a Microsoft Azure API Management developer portal (\"Discover APIs,\n    learn how to use them, try them out interactively, and sign up to acquire keys\"), and\n    api.uwa.edu.au answers as a live APIM gateway (HTTP/2 404, content-type application/json,\n    Azure request-context header). Azure APIM's subscription-key header is the platform default.\n    Marked medium confidence because the product catalog is behind sign-in — the specific header\n    name and any per-product override could not be read without an account, and /signup returns\n    404. No key was obtained and no protected operation was called.\n  sources:\n  - https://api-portal.uwa.edu.au/\n  - https://api.uwa.edu.au/\n- name: shibboleth-saml2\n  type: saml2\n  surface: uwa:identity-federation\n\
  \  x-operator: institution\n  description: >-\n    UWA operates its own Shibboleth SAML 2.0 identity provider at\n    https://idp.uwa.edu.au/idp/shibboleth, scoped to uwa.edu.au, with HTTP-POST and HTTP-Redirect\n    SingleSignOnService bindings and transient NameID. This is the credential behind essentially\n    every affiliation-gated UWA service, and it is the institution's most significant\n    machine-readable, standards-based surface.\n  sources:\n  - https://idp.uwa.edu.au/idp/shibboleth\nnot_assessed:\n- surface: Elsevier Pure Web Service (api.research-repository.uwa.edu.au/ws/api/524)\n  x-operator: tenant\n  reason: >-\n    Requires a Pure API key issued from the Pure Administrator tab. The contract is Elsevier's\n    (\"Pure Web Service 524\", info.contact.name \"Elsevier\"), so its auth model is Elsevier's\n    engineering and belongs to the Elsevier repo, not to UWA's.\n- surface: Ex Libris Primo VE (onesearch.library.uwa.edu.au)\n  x-operator: tenant\n  reason: Ex Libris\
  \ product; UWA is tenant 61UWA_INST. Auth model is Ex Libris's.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uwa/refs/heads/main/authentication/uwa-authentication.yml
summary_line: none/apiKey/saml2 · 3 schemes
tags:
- Education
- Higher Education
- University
- Australia
- Group of Eight
- Perth
- Research
- Research Data
- Research Repository
- Identity Federation
- OAI-PMH
- Library
---
