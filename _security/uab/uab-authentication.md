---
api_key_in: []
api_specs:
- filename: uab-ddd-openapi.yml
  format: yaml
  label: DDD — Dipòsit Digital de Documents de la UAB (OAI-PMH 2.0)
  slug: ddd-oai-pmh
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uab/refs/heads/main/openapi/uab-ddd-openapi.yml
- filename: uab-ddd-openapi.yml
  format: yaml
  label: DDD Invenio Search and Export Interface
  slug: ddd-search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uab/refs/heads/main/openapi/uab-ddd-openapi.yml
auth_types: []
description: UAB's programmable surface splits cleanly in two on authentication. Everything that carries scholarly metadata out of the institution — OAI-PMH harvesting and Invenio export at ddd, traces, ifmuc and the journal platform — is open and anonymous, with no key, no registration and no quota published. Everything that touches a person is behind the institution's own Apereo CAS server, which speaks CAS 3.0 to UAB applications and SAML 2.0 to federated relying parties. There is no API-key programme, no OAuth authorization server for third-party developers, and no self-service developer registration anywhere on the estate.
kind: authentication
layout: security
method: probed
name: Uab Authentication
name_suffix: Authentication
oauth_flows: []
overview: Autonomous University of Barcelona declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Autonomous University of Barcelona
provider_slug: uab
scheme_count: 0
schemes: []
slug: uab-authentication
source_filename: uab-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "specification: API Commons Authentication\nspecificationVersion: '0.1'\nprovider: Autonomous University of Barcelona\nproviderId: uab\ngenerated: '2026-09-01'\nmethod: probed\nsource: >-\n  Live probes on 2026-09-01 of https://ddd.uab.cat/oai2d, https://ddd.uab.cat/search,\n  https://sso.uab.cat/cas/login, https://sso.uab.cat/cas/p3/serviceValidate,\n  https://sso.uab.cat/cas/idp/metadata and https://dataverse.csuc.cat/api/dataverses/UAB.\ndescription: >-\n  UAB's programmable surface splits cleanly in two on authentication. Everything that\n  carries scholarly metadata out of the institution — OAI-PMH harvesting and Invenio\n  export at ddd, traces, ifmuc and the journal platform — is open and anonymous, with no\n  key, no registration and no quota published. Everything that touches a person is behind\n  the institution's own Apereo CAS server, which speaks CAS 3.0 to UAB applications and\n  SAML 2.0 to federated relying parties. There is no API-key programme, no OAuth\n \
  \ authorization server for third-party developers, and no self-service developer\n  registration anywhere on the estate.\n\nmechanisms:\n- name: Anonymous\n  applies_to:\n  - uab:ddd-oai-pmh\n  - uab:ddd-search\n  - uab:traces-oai-pmh\n  - uab:ifmuc-oai-pmh\n  - uab:revistes-ojs-oai\n  x-operator: institution\n  type: none\n  evidence:\n    url: https://ddd.uab.cat/oai2d?verb=Identify\n    status: 200\n    note: >-\n      Served without credentials, without a cookie and without a rate-limit header. The\n      Identify response's metadataPolicy declares free and unlimited use of records under\n      CC0 1.0; the dataPolicy notes that access to full text may be free, embargoed or\n      restricted to the UAB domain, and that submission is restricted.\n\n- name: CAS 3.0 ticket validation\n  applies_to:\n  - uab:sso-cas\n  x-operator: institution\n  type: ticket\n  endpoints:\n    login: https://sso.uab.cat/cas/login\n    validate: https://sso.uab.cat/cas/p3/serviceValidate\n    logout: https://sso.uab.cat/cas/logout\n\
  \  evidence:\n    url: 'https://sso.uab.cat/cas/p3/serviceValidate?service=https://example.org&ticket=ST-invalid'\n    status: 403\n    body: >-\n      <cas:serviceResponse><cas:authenticationFailure code=\"INVALID_TICKET\">No se ha\n      reconocido el tique 'ST-invalid'</cas:authenticationFailure></cas:serviceResponse>\n    note: >-\n      A well-formed CAS protocol rejection of a deliberately invalid ticket — evidence the\n      validation endpoint is live and speaking the protocol, not evidence of any access\n      granted. Service registration is administrative; there is no self-service path.\n\n- name: SAML 2.0 web browser SSO\n  applies_to:\n  - uab:sso-saml-idp\n  - uab:sir-federation-entity\n  x-operator: institution\n  type: saml\n  metadata: https://sso.uab.cat/cas/idp/metadata\n  entity_id: https://sso.uab.cat/cas/idp\n  bindings:\n  - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST\n  - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST-SimpleSign\n  - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect\n\
  \  - urn:oasis:names:tc:SAML:2.0:bindings:SOAP\n  evidence:\n    url: https://sso.uab.cat/cas/idp/metadata\n    status: 200\n    note: >-\n      Signing and encryption key descriptors both present. Federated relying parties reach\n      UAB either directly against this entity or through the RedIRIS SIR gateway entity\n      https://www.rediris.es/sir/uabidp, which is federation-operated and detailed in\n      identity-federation/uab-identity-federation.yml.\n\n- name: Dataverse API token\n  applies_to:\n  - uab:cora-rdr\n  x-operator: tenant\n  type: apiKey\n  in: header\n  parameter_name: X-Dataverse-key\n  evidence:\n    url: https://dataverse.csuc.cat/api/dataverses/UAB\n    status: 200\n    note: >-\n      Read access to UAB's collection is anonymous; write access uses the X-Dataverse-key\n      header advertised in the platform's CORS Access-Control-Allow-Headers. This scheme is\n      CSUC's and Dataverse's, recorded here because it is how UAB's research data is\n      reached —\
  \ not because UAB designed it.\n\nabsent:\n- mechanism: oauth2\n  note: No authorization server, no /.well-known/oauth-authorization-server, no consent screen on any UAB host.\n- mechanism: apiKey\n  note: No API-key issuance, developer registration or key-management page exists on any UAB host.\n- mechanism: openid_connect\n  note: >-\n    Apereo CAS can serve OIDC, but the module is not exposed here:\n    https://sso.uab.cat/cas/oidc/.well-known/openid-configuration returns 404,\n    https://sso.uab.cat/.well-known/openid-configuration returns 404, and\n    https://sso.uab.cat/cas/oidc/jwks returns a CAS 404 error document. Probed\n    2026-09-01.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uab/refs/heads/main/authentication/uab-authentication.yml
summary_line: 0 schemes
tags:
- Education
- Higher Education
- University
- Spain
- Catalonia
- Research
- Open Access
- Institutional Repository
- Research Repository
- Research Data
- OAI-PMH
- Identity Federation
- Scholarly Publishing
---
