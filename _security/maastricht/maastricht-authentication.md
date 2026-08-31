---
api_key_in: []
api_specs:
- filename: maastricht-oai-pmh-openapi.yml
  format: yaml
  label: Maastricht University Research Portal OAI-PMH
  slug: oai-pmh
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maastricht/refs/heads/main/openapi/maastricht-oai-pmh-openapi.yml
auth_types: []
description: Authentication surfaces Maastricht University itself operates. The institution runs its own identity provider (Microsoft ADFS) on its own registrable domain and publishes BOTH an OIDC discovery document and signed SAML 2.0 federation metadata without authentication — a genuinely machine-readable, institution-operated surface, and the one class of university API that is almost never catalogued.
kind: authentication
layout: security
method: probed
name: Maastricht Authentication
name_suffix: Authentication
oauth_flows: []
overview: Maastricht University declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Maastricht University
provider_slug: maastricht
scheme_count: 0
schemes: []
slug: maastricht-authentication
source_filename: maastricht-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "provider: Maastricht University\nproviderId: maastricht\ngenerated: '2026-08-30'\nmethod: probed\nsource: >-\n  https://login.maastrichtuniversity.nl/adfs/.well-known/openid-configuration (200),\n  https://login.maastrichtuniversity.nl/FederationMetadata/2007-06/FederationMetadata.xml (200),\n  https://metadata.surfconext.nl/idps-metadata.xml (200), all fetched 2026-08-30.\ndescription: >-\n  Authentication surfaces Maastricht University itself operates. The institution runs its own\n  identity provider (Microsoft ADFS) on its own registrable domain and publishes BOTH an OIDC\n  discovery document and signed SAML 2.0 federation metadata without authentication — a genuinely\n  machine-readable, institution-operated surface, and the one class of university API that is\n  almost never catalogued.\nsurfaces:\n- id: adfs-oidc\n  name: Maastricht University ADFS — OpenID Connect discovery\n  operator: institution\n  protocol: OpenID Connect 1.0 / OAuth 2.0\n  issuer: https://login.maastrichtuniversity.nl/adfs\n\
  \  discovery: https://login.maastrichtuniversity.nl/adfs/.well-known/openid-configuration\n  status: 200\n  public: true\n  endpoints:\n    authorization: https://login.maastrichtuniversity.nl/adfs/oauth2/authorize/\n    token: https://login.maastrichtuniversity.nl/adfs/oauth2/token/\n    userinfo: https://login.maastrichtuniversity.nl/adfs/userinfo\n    jwks: https://login.maastrichtuniversity.nl/adfs/discovery/keys\n    end_session: https://login.maastrichtuniversity.nl/adfs/oauth2/logout\n  grant_types:\n  - authorization_code\n  - refresh_token\n  - client_credentials\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  - urn:ietf:params:oauth:grant-type:device_code\n  - implicit\n  - password\n  token_endpoint_auth_methods:\n  - client_secret_post\n  - client_secret_basic\n  - private_key_jwt\n  - windows_client_authentication\n  id_token_signing_alg: [RS256]\n  frontchannel_logout_supported: true\n  registration: >-\n    Client registration is not self-service. There is no public\
  \ dynamic-registration endpoint;\n    relying-party trusts are provisioned by UM ICT Services for institutionally affiliated\n    applications.\n- id: adfs-saml\n  name: Maastricht University ADFS — SAML 2.0 identity provider\n  operator: institution\n  protocol: SAML 2.0 Web Browser SSO\n  entity_id: http://login.maastrichtuniversity.nl/adfs/services/trust\n  metadata: https://login.maastrichtuniversity.nl/FederationMetadata/2007-06/FederationMetadata.xml\n  status: 200\n  content_type: application/samlmetadata+xml\n  public: true\n  name_id_formats:\n  - urn:oasis:names:tc:SAML:2.0:nameid-format:persistent\n  - urn:oasis:names:tc:SAML:2.0:nameid-format:transient\n- id: surfconext-federation\n  name: SURFconext / eduGAIN federation entry\n  operator: tenant\n  detail: >-\n    Maastricht's IdP entity is published in the Dutch national research-and-education federation\n    operated by SURF, which is connected to eduGAIN. SURF operates the federation and the proxy\n    (engine.surfconext.nl);\
  \ Maastricht operates the entity inside it.\n  metadata: https://metadata.surfconext.nl/idps-metadata.xml\n  status: 200\n  scopes:\n  - maastrichtuniversity.nl\n  - unimaas.nl\n  display_name: Maastricht University\n  sso_location: https://engine.surfconext.nl/authentication/idp/single-sign-on/key:20230503/cce637f0ae222246ad62a8590d25fa9d\n- id: oai-anonymous\n  name: OAI-PMH harvesting — no authentication\n  operator: institution\n  protocol: none\n  detail: >-\n    https://cris.maastrichtuniversity.nl/ws/oai is keyless and requires no registration. All six\n    verbs returned 200 anonymously on 2026-08-30.\n- id: pure-ws-api\n  name: Pure REST API — key-gated\n  operator: tenant\n  protocol: api-key\n  detail: >-\n    https://cris.maastrichtuniversity.nl/ws/api returns Elsevier's Pure API documentation\n    (canonical https://api.elsevierpure.com/ws/api/documentation/index.html) and\n    /ws/api/524/openapi.yaml returns 401. The contract is Elsevier's; keys are issued by UM to\n   \
  \ affiliated consumers. Not credited as an institution-authored API.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/maastricht/refs/heads/main/authentication/maastricht-authentication.yml
summary_line: 0 schemes
tags:
- University
- Higher Education
- Education
- Netherlands
- Europe
- Research Data
- Research Repository
- Identity Federation
- OAI-PMH
- Open Access
- Public Research University
---
