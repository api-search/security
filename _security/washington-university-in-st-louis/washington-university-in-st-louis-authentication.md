---
api_key_in: []
auth_types: []
description: 'How Washington University''s machine-readable surfaces authenticate. Four distinct regimes are in play, and only one of them is an ordinary API credential. CIViC — the institution''s genuinely public API — reads anonymously and takes an optional bearer API key for writes and for a higher rate ceiling. The enterprise integration APIs on MuleSoft Anypoint are not self-service at all: access is granted by an internal ServiceNow request and is scoped to WashU integrators. The two research repositories harvest anonymously over OAI-PMH. And the institution''s Shibboleth IdP is federation infrastructure for browser sign-on, not an API credential — it is recorded here because it is the gate behind every one of WashU''s auth-walled research systems.'
kind: authentication
layout: security
method: probed
name: Washington University In St Louis Authentication
name_suffix: Authentication
oauth_flows: []
overview: Washington University in St. Louis declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Washington University in St. Louis
provider_slug: washington-university-in-st-louis
scheme_count: 0
schemes: []
slug: washington-university-in-st-louis-authentication
source_filename: washington-university-in-st-louis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "---\nname: Washington University in St. Louis — Authentication\ndescription: >-\n  How Washington University's machine-readable surfaces authenticate. Four distinct regimes are in\n  play, and only one of them is an ordinary API credential. CIViC — the institution's genuinely\n  public API — reads anonymously and takes an optional bearer API key for writes and for a higher\n  rate ceiling. The enterprise integration APIs on MuleSoft Anypoint are not self-service at all:\n  access is granted by an internal ServiceNow request and is scoped to WashU integrators. The two\n  research repositories harvest anonymously over OAI-PMH. And the institution's Shibboleth IdP is\n  federation infrastructure for browser sign-on, not an API credential — it is recorded here because\n  it is the gate behind every one of WashU's auth-walled research systems.\ngenerated: '2026-09-01'\nx-method: derived\nx-authorship: This file is our writing; the mechanisms are quoted from operator docs and live\
  \ probes.\nmethod: probed\nsource: >-\n  https://docs.civicdb.org/en/latest/api.html (operator documentation), plus live unauthenticated\n  probes of civicdb.org/api/graphql, cnda.wustl.edu, balsa.wustl.edu, the two OAI-PMH endpoints and\n  mdq.incommon.org on 2026-09-01.\nx-operator: institution\nurl: https://raw.githubusercontent.com/api-evangelist/washington-university-in-st-louis/main/authentication/washington-university-in-st-louis-authentication.yml\n\nmechanisms:\n  - id: civic-bearer-api-key\n    type: http\n    scheme: bearer\n    label: CIViC API key as an HTTP bearer token\n    in: header\n    parameter_names:\n      - Authorization\n    applies_to:\n      - CIViC GraphQL API (https://civicdb.org/api/graphql)\n    anonymous_access: >-\n      Yes for reads. An unauthenticated POST of a standard introspection query returned HTTP 200 and\n      the full 502-type schema on 2026-09-01; no credential was presented or required.\n    required_for:\n      - All 47 GraphQL mutations (curation,\
  \ moderation, revision, key management)\n      - Any client that needs to exceed the anonymous rate ceiling\n    onboarding: >-\n      Sign in to civicdb.org, open the user profile, choose \"Manage API Keys\" and click \"Generate\n      New API Key\". The full token is displayed once at creation; afterwards the list shows only a\n      masked reminder. Keys are revocable, and a key can also be minted or revoked through the API\n      itself via the generateApiKey and revokeApiKey mutations.\n    header_form: 'Authorization: Bearer <CIVIC_API_KEY>'\n    operator_guidance: >-\n      The operator documents explicitly that keys must not be placed in URLs, query strings,\n      checked-in scripts or shared notebooks, and directs callers to environment variables or a\n      secrets manager for automated clients. It also asks that any key which is no longer needed or\n      may have been exposed be revoked.\n    cost: Free. The operator describes the key as \"(free)\".\n    method: searched\n\
  \    source: https://docs.civicdb.org/en/latest/api.html\n\n  - id: anypoint-servicenow-request\n    type: gated\n    label: WashU enterprise APIs — access by internal request, no public sign-up\n    applies_to:\n      - WashU enterprise integration APIs published in MuleSoft Anypoint Exchange\n    anonymous_access: >-\n      No. The portal pages describing the program are public (HTTP 200), but no endpoint, no\n      specification and no credential-issuing flow is reachable without an internal request.\n    onboarding: >-\n      A WashU integrator requests Anypoint Exchange access through ServiceNow; the process is\n      documented at https://data.wustl.edu/api-portal/api-portal-anypoint-access/. There is no\n      public developer sign-up, no self-service key, and no published client-registration endpoint.\n    audience: WashU faculty, staff and institutional integrators — not the general public.\n    method: searched\n    source: https://data.wustl.edu/api-portal/api-portal-anypoint-access/\n\
  \n  - id: oai-pmh-anonymous\n    type: none\n    label: OAI-PMH metadata harvesting — no credential\n    applies_to:\n      - https://openscholarship.wustl.edu/do/oai/\n      - https://digitalcommonsdata.wustl.edu/oai\n    anonymous_access: >-\n      Yes, fully. Identify, ListMetadataFormats and ListSets all returned HTTP 200 to an\n      unauthenticated request on 2026-09-01.\n    constraints: >-\n      The WashU Scholarly Repository publishes a data policy in its Identify response stating that\n      full content may not be harvested by robots without prior written approval; metadata itself is\n      explicitly open to commercial and non-commercial service providers.\n    method: probed\n    source: https://openscholarship.wustl.edu/do/oai/?verb=Identify\n\n  - id: xnat-and-balsa-session-login\n    type: gated\n    label: Research data platforms — interactive login, no anonymous API\n    applies_to:\n      - CNDA, the Central Neuroimaging Data Archive (https://cnda.wustl.edu)\n     \
  \ - BALSA neuroimaging database (https://balsa.wustl.edu)\n    anonymous_access: >-\n      No. Every CNDA path probed — including /data/version and /xapi/swagger.json, which are the\n      XNAT REST and OpenAPI endpoints — returns the same 23,725-byte login page at\n      /app/template/Login.vm with HTTP 200. That is a soft-200 gate, not an available contract:\n      the status code says success and the body is a sign-in form. balsa.wustl.edu is more honest\n      about it and returns a 302 to /login/auth.\n    note: >-\n      XNAT ships a real REST API and an OpenAPI document at /xapi/swagger.json, and the software\n      itself originated at WashU's Neuroinformatics Research Group. None of that contract is\n      publicly readable here, so none of it is saved under this profile.\n    method: probed\n    source: https://cnda.wustl.edu/xapi/swagger.json\n\n  - id: shibboleth-saml-idp\n    type: federation\n    label: WashU Shibboleth identity provider (InCommon)\n    entity_id: https://login.wustl.edu/idp/shibboleth\n\
  \    applies_to:\n      - Browser-based single sign-on to WashU services and to federated research services\n    protocols:\n      - SAML 2.0 (HTTP-POST and HTTP-Redirect SSO bindings)\n      - urn:mace:shibboleth:1.0 AuthnRequest profile\n    assurance:\n      - http://refeds.org/category/research-and-scholarship\n      - https://refeds.org/sirtfi\n    scope: wustl.edu\n    note: >-\n      This is not an API credential and no API in this profile accepts it directly. It is recorded\n      because it is the institution's own identity infrastructure — operated by WashU, published as\n      signed metadata in InCommon, and the gate standing in front of CNDA, BALSA and every Anypoint\n      consumer.\n    method: probed\n    source: https://mdq.incommon.org/entities/https%3A%2F%2Flogin.wustl.edu%2Fidp%2Fshibboleth\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/washington-university-in-st-louis/refs/heads/main/authentication/washington-university-in-st-louis-authentication.yml
summary_line: 0 schemes
tags:
- University
- Higher Education
- Education
- United States
- Missouri
- Private Research University
- Research Data
- Research Repository
- Identity Federation
- Genomics
- Bioinformatics
- GraphQL
- OAI-PMH
- Shibboleth
- DataCite
- MuleSoft
---
