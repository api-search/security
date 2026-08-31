---
api_key_in: []
api_specs:
- filename: kfupm-identity-federation-openapi.yml
  format: yaml
  label: KFUPM Identity Federation (SAML 2.0 + OpenID Connect)
  slug: identity-federation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kfupm/refs/heads/main/openapi/kfupm-identity-federation-openapi.yml
- filename: kfupm-eprints-oai-pmh-openapi.yml
  format: yaml
  label: KFUPM ePrints OAI-PMH Repository Interface
  slug: eprints-oai-pmh
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kfupm/refs/heads/main/openapi/kfupm-eprints-oai-pmh-openapi.yml
- filename: kfupm-eprints-export-openapi.yml
  format: yaml
  label: KFUPM ePrints Export & Search (JSON)
  slug: eprints-export
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kfupm/refs/heads/main/openapi/kfupm-eprints-export-openapi.yml
auth_types:
- openIdConnect
- oauth2
- saml2
- apiKey
- none
description: Authentication posture across KFUPM's surfaces. The previous version of this file described an api-key scheme derived from the Elsevier Pure Web Services OpenAPI; that contract is Elsevier's and has been removed from this repo, so this file was rebuilt from KFUPM's own identity provider.
kind: authentication
layout: security
method: probed
name: Kfupm Authentication
name_suffix: Authentication
oauth_flows: []
overview: King Fahd University of Petroleum & Minerals secures its APIs with openIdConnect, oauth2, saml2, apiKey, and none across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: King Fahd University of Petroleum & Minerals
provider_slug: kfupm
scheme_count: 4
schemes:
- client_auth_methods:
  - client_secret_post
  - client_secret_basic
  - private_key_jwt
  - windows_client_authentication
  description: Institution-operated OpenID Connect provider (Microsoft AD FS). Client registration is not self-serve — no public developer portal or client-registration endpoint was found; a relying party is onboarded by KFUPM IT.
  endpoints:
    authorization: https://sts.kfupm.edu.sa/adfs/oauth2/authorize/
    device_authorization: https://sts.kfupm.edu.sa/adfs/oauth2/devicecode
    end_session: https://sts.kfupm.edu.sa/adfs/oauth2/logout
    jwks: https://sts.kfupm.edu.sa/adfs/discovery/keys
    token: https://sts.kfupm.edu.sa/adfs/oauth2/token/
    userinfo: https://sts.kfupm.edu.sa/adfs/userinfo
  grant_types:
  - authorization_code
  - refresh_token
  - client_credentials
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  - urn:ietf:params:oauth:grant-type:device_code
  - implicit
  - password
  id_token_signing_alg: RS256
  issuer: https://sts.kfupm.edu.sa/adfs
  jwks_keys: 2
  name: kfupm-oidc
  openIdConnectUrl: https://sts.kfupm.edu.sa/adfs/.well-known/openid-configuration
  sources:
  - https://sts.kfupm.edu.sa/adfs/.well-known/openid-configuration
  subject_types:
  - pairwise
  type: openIdConnect
  x-operator: institution
- bindings:
  - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect
  - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST
  description: Institution-operated SAML 2.0 identity provider, registered in eduGAIN via MAEEN (SA-MIF) as entity 671205 with scope kfupm.edu.sa.
  entity_id: http://sts.kfupm.edu.sa/adfs/services/trust
  metadata_url: https://sts.kfupm.edu.sa/FederationMetadata/2007-06/FederationMetadata.xml
  name: kfupm-saml2
  nameid_formats:
  - urn:oasis:names:tc:SAML:2.0:nameid-format:persistent
  - urn:oasis:names:tc:SAML:2.0:nameid-format:transient
  - urn:oasis:names:tc:SAML:1.1:nameid-format:emailAddress
  sources:
  - https://sts.kfupm.edu.sa/FederationMetadata/2007-06/FederationMetadata.xml
  - https://technical.edugain.org/api.php?action=list_entities&format=json
  sso_endpoint: https://sts.kfupm.edu.sa/adfs/ls/
  type: saml2
  x-operator: institution
- description: The KFUPM ePrints OAI-PMH, JSON export and JSON search endpoints require no credential. Verified anonymous on 2026-08-30.
  name: eprints-anonymous
  sources:
  - https://eprints.kfupm.edu.sa/cgi/oai2?verb=Identify
  - https://eprints.kfupm.edu.sa/cgi/search/simple?q=petroleum&output=JSON
  type: none
  x-operator: institution
- description: The Elsevier Pure Web Services deployed at pure.kfupm.edu.sa authenticates with a Pure API key in an `api-key` header. This is Elsevier's scheme on Elsevier's contract; KFUPM operates the tenant, not the interface. Keys are issued from Pure administration, which redirects to https://pure.kfupm.edu.sa/admin/saml2/authenticate/pure — the tenant is itself fronted by KFUPM's SAML IdP.
  in: header
  name: pure-ws-api-key
  parameter: api-key
  sources:
  - https://pure.kfupm.edu.sa/ws/api/
  type: apiKey
  x-operator: tenant
slug: kfupm-authentication
source_filename: kfupm-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: >-\n  https://sts.kfupm.edu.sa/adfs/.well-known/openid-configuration (200),\n  https://sts.kfupm.edu.sa/adfs/discovery/keys (200),\n  https://sts.kfupm.edu.sa/FederationMetadata/2007-06/FederationMetadata.xml (200),\n  https://pure.kfupm.edu.sa/ws/api/ (200) — probed 2026-08-30.\nprovider: King Fahd University of Petroleum & Minerals\nproviderId: kfupm\ndescription: >-\n  Authentication posture across KFUPM's surfaces. The previous version of this file described an\n  api-key scheme derived from the Elsevier Pure Web Services OpenAPI; that contract is Elsevier's\n  and has been removed from this repo, so this file was rebuilt from KFUPM's own identity provider.\nsummary:\n  types: [openIdConnect, oauth2, saml2, apiKey, none]\n  institution_operated: [openIdConnect, oauth2, saml2, none]\n  tenant_operated: [apiKey]\nschemes:\n  - name: kfupm-oidc\n    type: openIdConnect\n    x-operator: institution\n    openIdConnectUrl: https://sts.kfupm.edu.sa/adfs/.well-known/openid-configuration\n\
  \    issuer: https://sts.kfupm.edu.sa/adfs\n    description: >-\n      Institution-operated OpenID Connect provider (Microsoft AD FS). Client registration is not\n      self-serve — no public developer portal or client-registration endpoint was found; a\n      relying party is onboarded by KFUPM IT.\n    endpoints:\n      authorization: https://sts.kfupm.edu.sa/adfs/oauth2/authorize/\n      token: https://sts.kfupm.edu.sa/adfs/oauth2/token/\n      userinfo: https://sts.kfupm.edu.sa/adfs/userinfo\n      jwks: https://sts.kfupm.edu.sa/adfs/discovery/keys\n      end_session: https://sts.kfupm.edu.sa/adfs/oauth2/logout\n      device_authorization: https://sts.kfupm.edu.sa/adfs/oauth2/devicecode\n    grant_types:\n      - authorization_code\n      - refresh_token\n      - client_credentials\n      - urn:ietf:params:oauth:grant-type:jwt-bearer\n      - urn:ietf:params:oauth:grant-type:device_code\n      - implicit\n      - password\n    client_auth_methods:\n      - client_secret_post\n    \
  \  - client_secret_basic\n      - private_key_jwt\n      - windows_client_authentication\n    id_token_signing_alg: RS256\n    subject_types: [pairwise]\n    jwks_keys: 2\n    sources:\n      - https://sts.kfupm.edu.sa/adfs/.well-known/openid-configuration\n  - name: kfupm-saml2\n    type: saml2\n    x-operator: institution\n    description: >-\n      Institution-operated SAML 2.0 identity provider, registered in eduGAIN via MAEEN (SA-MIF)\n      as entity 671205 with scope kfupm.edu.sa.\n    entity_id: http://sts.kfupm.edu.sa/adfs/services/trust\n    metadata_url: https://sts.kfupm.edu.sa/FederationMetadata/2007-06/FederationMetadata.xml\n    sso_endpoint: https://sts.kfupm.edu.sa/adfs/ls/\n    bindings:\n      - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect\n      - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST\n    nameid_formats:\n      - urn:oasis:names:tc:SAML:2.0:nameid-format:persistent\n      - urn:oasis:names:tc:SAML:2.0:nameid-format:transient\n      - urn:oasis:names:tc:SAML:1.1:nameid-format:emailAddress\n\
  \    sources:\n      - https://sts.kfupm.edu.sa/FederationMetadata/2007-06/FederationMetadata.xml\n      - https://technical.edugain.org/api.php?action=list_entities&format=json\n  - name: eprints-anonymous\n    type: none\n    x-operator: institution\n    description: >-\n      The KFUPM ePrints OAI-PMH, JSON export and JSON search endpoints require no credential.\n      Verified anonymous on 2026-08-30.\n    sources:\n      - https://eprints.kfupm.edu.sa/cgi/oai2?verb=Identify\n      - https://eprints.kfupm.edu.sa/cgi/search/simple?q=petroleum&output=JSON\n  - name: pure-ws-api-key\n    type: apiKey\n    in: header\n    parameter: api-key\n    x-operator: tenant\n    description: >-\n      The Elsevier Pure Web Services deployed at pure.kfupm.edu.sa authenticates with a Pure API\n      key in an `api-key` header. This is Elsevier's scheme on Elsevier's contract; KFUPM operates\n      the tenant, not the interface. Keys are issued from Pure administration, which redirects to\n      https://pure.kfupm.edu.sa/admin/saml2/authenticate/pure\
  \ — the tenant is itself fronted by\n      KFUPM's SAML IdP.\n    sources:\n      - https://pure.kfupm.edu.sa/ws/api/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kfupm/refs/heads/main/authentication/kfupm-authentication.yml
summary_line: openIdConnect/oauth2/saml2/apiKey/none · 4 schemes
tags:
- University
- Higher Education
- Education
- Research
- Saudi Arabia
- Middle East
- Identity Federation
- Research Repository
- Open Access
- OAI-PMH
- Theses
- Course Catalog
---
