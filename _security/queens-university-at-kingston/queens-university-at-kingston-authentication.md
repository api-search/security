---
api_key_in: []
auth_types:
- saml2
description: ''
kind: authentication
layout: security
method: probed
name: Queens University At Kingston Authentication
name_suffix: Authentication
oauth_flows: []
overview: Queen's University at Kingston secures its APIs with saml2 across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Queen's University at Kingston
provider_slug: queens-university-at-kingston
scheme_count: 3
schemes:
- detail: IdP metadata is served as application/xml at a stable, unauthenticated URL, carrying an IDPSSODescriptor, an X509 signing certificate, and a shibmd:Scope of queensu.ca. This is the credential surface every federated Queen's service — including its repository tenants — resolves to.
  documented: true
  entity_id: https://login.queensu.ca/idp/shibboleth
  metadata_url: https://login.queensu.ca/idp/shibboleth
  name: Shibboleth / SAML 2.0 Single Sign-On
  protocol_support: urn:oasis:names:tc:SAML:2.0:protocol
  scope: queensu.ca
  type: saml2
  x-operator: institution
- detail: 'The Queen''s institutional repository REST API answers unauthenticated requests with `WWW-Authenticate: password realm="DSpace REST API", shibboleth realm="DSpace REST API", ip realm="DSpace REST API"` and a Shibboleth login location. Read access to public records needs no credential at all. The scheme is DSpace''s, deployed by OCUL / Scholars Portal.'
  documented: true
  evidence:
  - locator: WWW-Authenticate response header
    url: https://queensu.scholaris.ca/server/api/authn/status
  name: DSpace REST API authentication (QSpace on Scholaris)
  type: multiple
  x-operator: tenant
- detail: Deposit and management operations against the Queen's University Dataverse Collection use a Dataverse API token passed in the X-Dataverse-key header. Tokens are issued by Borealis, not by Queen's; public search and metadata reads are keyless.
  docs: https://borealisdata.ca/guides/en/latest/api/native-api.html
  documented: true
  name: Dataverse API token (Queen's collection on Borealis)
  type: apiKey
  x-operator: tenant
slug: queens-university-at-kingston-authentication
source_filename: queens-university-at-kingston-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: >-\n  https://login.queensu.ca/idp/shibboleth (SAML 2.0 IdP metadata) and\n  https://queensu.scholaris.ca/server/api/authn/status (WWW-Authenticate challenge), probed 2026-08-30\nprovider: Queen's University at Kingston\nproviderId: queens-university-at-kingston\nnote: >-\n  Queen's publishes no public API key, OAuth application registration, or developer credential flow of\n  its own — there is no institution-operated public API to authenticate against. What it does operate,\n  and publish machine-readably, is federated identity: a Shibboleth Identity Provider on its own domain\n  serving SAML 2.0 metadata. That is the institution's real authentication surface and the one recorded\n  here. The token flows of its repository tenants belong to the platforms that run them (DSpace on\n  Scholaris, Dataverse on Borealis) and are not restated as Queen's own.\nsummary:\n  types:\n  - saml2\n  api_key_in: []\n  oauth2_flows: []\n  self_service_signup:\
  \ false\nschemes:\n- name: Shibboleth / SAML 2.0 Single Sign-On\n  type: saml2\n  x-operator: institution\n  documented: true\n  entity_id: https://login.queensu.ca/idp/shibboleth\n  metadata_url: https://login.queensu.ca/idp/shibboleth\n  scope: queensu.ca\n  protocol_support: urn:oasis:names:tc:SAML:2.0:protocol\n  detail: >-\n    IdP metadata is served as application/xml at a stable, unauthenticated URL, carrying an\n    IDPSSODescriptor, an X509 signing certificate, and a shibmd:Scope of queensu.ca. This is the\n    credential surface every federated Queen's service — including its repository tenants — resolves to.\n- name: DSpace REST API authentication (QSpace on Scholaris)\n  type: multiple\n  x-operator: tenant\n  documented: true\n  detail: >-\n    The Queen's institutional repository REST API answers unauthenticated requests with\n    `WWW-Authenticate: password realm=\"DSpace REST API\", shibboleth realm=\"DSpace REST API\",\n    ip realm=\"DSpace REST API\"` and a Shibboleth\
  \ login location. Read access to public records needs no\n    credential at all. The scheme is DSpace's, deployed by OCUL / Scholars Portal.\n  evidence:\n  - url: https://queensu.scholaris.ca/server/api/authn/status\n    locator: WWW-Authenticate response header\n- name: Dataverse API token (Queen's collection on Borealis)\n  type: apiKey\n  x-operator: tenant\n  documented: true\n  detail: >-\n    Deposit and management operations against the Queen's University Dataverse Collection use a\n    Dataverse API token passed in the X-Dataverse-key header. Tokens are issued by Borealis, not by\n    Queen's; public search and metadata reads are keyless.\n  docs: https://borealisdata.ca/guides/en/latest/api/native-api.html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/queens-university-at-kingston/refs/heads/main/authentication/queens-university-at-kingston-authentication.yml
summary_line: saml2 · 3 schemes
tags:
- University
- Higher Education
- Education
- Canada
- Ontario
- U15
- Public Research University
- Research Data
- Institutional Repository
- Identity Federation
- OAI-PMH
- Library
---
