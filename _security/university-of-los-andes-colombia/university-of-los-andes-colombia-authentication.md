---
api_key_in: []
api_specs:
- filename: university-of-los-andes-colombia-revistas-oai-pmh-openapi.yml
  format: yaml
  label: Revistas Uniandes - OAI-PMH
  slug: revistas-oai
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-los-andes-colombia/refs/heads/main/openapi/university-of-los-andes-colombia-revistas-oai-pmh-openapi.yml
auth_types:
- openIdConnect
- saml2
- none
description: ''
kind: authentication
layout: security
method: probed
name: University Of Los Andes Colombia Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Los Andes Colombia secures its APIs with openIdConnect, saml2, and none across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: University of Los Andes Colombia
provider_slug: university-of-los-andes-colombia
scheme_count: 3
schemes:
- description: OpenID Connect discovery for the institution's Entra ID tenant. Resolvable by the university's own domain name as well as by tenant GUID; both return issuer https://login.microsoftonline.com/fabd047c-ff48-492a-8bbb-8f98b9fb9cca/v2.0.
  details:
    authorization_endpoint: https://login.microsoftonline.com/fabd047c-ff48-492a-8bbb-8f98b9fb9cca/oauth2/v2.0/authorize
    issuer: https://login.microsoftonline.com/fabd047c-ff48-492a-8bbb-8f98b9fb9cca/v2.0
    jwks_uri: https://login.microsoftonline.com/fabd047c-ff48-492a-8bbb-8f98b9fb9cca/discovery/v2.0/keys
    scopes_supported:
    - openid
    - profile
    - email
    - offline_access
    tenant_id: fabd047c-ff48-492a-8bbb-8f98b9fb9cca
    tenant_region_scope: SA
    token_endpoint: https://login.microsoftonline.com/fabd047c-ff48-492a-8bbb-8f98b9fb9cca/oauth2/v2.0/token
  evidence:
    bytes: 1964
    status: 200
    url: https://login.microsoftonline.com/uniandes.edu.co/v2.0/.well-known/openid-configuration
  name: entraIdOidc
  openIdConnectUrl: https://login.microsoftonline.com/uniandes.edu.co/v2.0/.well-known/openid-configuration
  operator: federation
  sources:
  - https://login.microsoftonline.com/uniandes.edu.co/v2.0/.well-known/openid-configuration
  type: openIdConnect
- description: 'SAML 2.0 identity provider for uniandes.edu.co. Tenant ownership confirmed by getuserrealm.srf, which returns FederationBrandName `Universidad de los Andes`, DomainName `uniandes.edu.co`, NameSpaceType `Managed`. Observed in production use: the Brightspace LMS at bloqueneon.uniandes.edu.co redirects unauthenticated visitors to this tenant''s /saml2 endpoint with a SAMLRequest.'
  details:
    entity_id: https://sts.windows.net/fabd047c-ff48-492a-8bbb-8f98b9fb9cca/
    metadata_url: https://login.microsoftonline.com/fabd047c-ff48-492a-8bbb-8f98b9fb9cca/federationmetadata/2007-06/federationmetadata.xml
    single_sign_on_service:
    - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect
      location: https://login.microsoftonline.com/fabd047c-ff48-492a-8bbb-8f98b9fb9cca/saml2
    - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST
      location: https://login.microsoftonline.com/fabd047c-ff48-492a-8bbb-8f98b9fb9cca/saml2
  evidence:
    bytes: 28441
    status: 200
    url: https://login.microsoftonline.com/fabd047c-ff48-492a-8bbb-8f98b9fb9cca/federationmetadata/2007-06/federationmetadata.xml
  name: entraIdSaml2
  operator: federation
  sources:
  - https://login.microsoftonline.com/fabd047c-ff48-492a-8bbb-8f98b9fb9cca/federationmetadata/2007-06/federationmetadata.xml
  - https://login.microsoftonline.com/getuserrealm.srf?login=user@uniandes.edu.co&json=1
  type: saml2
- description: The OAI-PMH endpoint at revistas.uniandes.edu.co takes no credential — all six verbs return data to anonymous clients. This is the only Uniandes surface found that serves an automated client without a credential or a challenge.
  name: none
  operator: institution
  sources:
  - openapi/university-of-los-andes-colombia-revistas-oai-pmh-openapi.yml
  type: none
slug: university-of-los-andes-colombia-authentication
source_filename: university-of-los-andes-colombia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: probed\nsource:\n- https://login.microsoftonline.com/uniandes.edu.co/v2.0/.well-known/openid-configuration\n- https://login.microsoftonline.com/fabd047c-ff48-492a-8bbb-8f98b9fb9cca/federationmetadata/2007-06/federationmetadata.xml\n- https://login.microsoftonline.com/getuserrealm.srf?login=user@uniandes.edu.co&json=1\n- https://revistas.uniandes.edu.co/index.php/index/api/v1/contexts\nnote: >-\n  Universidad de los Andes publishes no developer portal, no API key programme and no documented\n  authentication model for any public API. What it does operate is an institutional identity\n  provider — a Microsoft Entra ID tenant fronting uniandes.edu.co — whose SAML 2.0 and OpenID\n  Connect discovery documents are publicly machine-readable. Those are recorded below because they\n  are the institution's own identity surface, not because they authenticate a public API. The one\n  anonymous-readable institution surface (the OAI-PMH endpoint) requires\
  \ no authentication at all.\nsummary:\n  types:\n  - openIdConnect\n  - saml2\n  - none\nschemes:\n- name: entraIdOidc\n  type: openIdConnect\n  operator: federation\n  openIdConnectUrl: https://login.microsoftonline.com/uniandes.edu.co/v2.0/.well-known/openid-configuration\n  description: >-\n    OpenID Connect discovery for the institution's Entra ID tenant. Resolvable by the university's\n    own domain name as well as by tenant GUID; both return issuer\n    https://login.microsoftonline.com/fabd047c-ff48-492a-8bbb-8f98b9fb9cca/v2.0.\n  evidence:\n    url: https://login.microsoftonline.com/uniandes.edu.co/v2.0/.well-known/openid-configuration\n    status: 200\n    bytes: 1964\n  details:\n    issuer: https://login.microsoftonline.com/fabd047c-ff48-492a-8bbb-8f98b9fb9cca/v2.0\n    tenant_id: fabd047c-ff48-492a-8bbb-8f98b9fb9cca\n    tenant_region_scope: SA\n    authorization_endpoint: https://login.microsoftonline.com/fabd047c-ff48-492a-8bbb-8f98b9fb9cca/oauth2/v2.0/authorize\n    token_endpoint:\
  \ https://login.microsoftonline.com/fabd047c-ff48-492a-8bbb-8f98b9fb9cca/oauth2/v2.0/token\n    jwks_uri: https://login.microsoftonline.com/fabd047c-ff48-492a-8bbb-8f98b9fb9cca/discovery/v2.0/keys\n    scopes_supported:\n    - openid\n    - profile\n    - email\n    - offline_access\n  sources:\n  - https://login.microsoftonline.com/uniandes.edu.co/v2.0/.well-known/openid-configuration\n- name: entraIdSaml2\n  type: saml2\n  operator: federation\n  description: >-\n    SAML 2.0 identity provider for uniandes.edu.co. Tenant ownership confirmed by\n    getuserrealm.srf, which returns FederationBrandName `Universidad de los Andes`, DomainName\n    `uniandes.edu.co`, NameSpaceType `Managed`. Observed in production use: the Brightspace LMS at\n    bloqueneon.uniandes.edu.co redirects unauthenticated visitors to this tenant's /saml2 endpoint\n    with a SAMLRequest.\n  evidence:\n    url: https://login.microsoftonline.com/fabd047c-ff48-492a-8bbb-8f98b9fb9cca/federationmetadata/2007-06/federationmetadata.xml\n\
  \    status: 200\n    bytes: 28441\n  details:\n    entity_id: https://sts.windows.net/fabd047c-ff48-492a-8bbb-8f98b9fb9cca/\n    metadata_url: https://login.microsoftonline.com/fabd047c-ff48-492a-8bbb-8f98b9fb9cca/federationmetadata/2007-06/federationmetadata.xml\n    single_sign_on_service:\n    - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect\n      location: https://login.microsoftonline.com/fabd047c-ff48-492a-8bbb-8f98b9fb9cca/saml2\n    - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST\n      location: https://login.microsoftonline.com/fabd047c-ff48-492a-8bbb-8f98b9fb9cca/saml2\n  sources:\n  - https://login.microsoftonline.com/fabd047c-ff48-492a-8bbb-8f98b9fb9cca/federationmetadata/2007-06/federationmetadata.xml\n  - https://login.microsoftonline.com/getuserrealm.srf?login=user@uniandes.edu.co&json=1\n- name: none\n  type: none\n  operator: institution\n  description: >-\n    The OAI-PMH endpoint at revistas.uniandes.edu.co takes no credential — all six verbs\
  \ return\n    data to anonymous clients. This is the only Uniandes surface found that serves an automated\n    client without a credential or a challenge.\n  sources:\n  - openapi/university-of-los-andes-colombia-revistas-oai-pmh-openapi.yml\ngated:\n- surface: OJS REST API (revistas.uniandes.edu.co/index.php/{journal}/api/v1)\n  operator: institution\n  status: 403\n  body: '{\"error\":\"api.403.unauthorized\",\"errorMessage\":\"No esta autorizado para acceder al recurso solicitado.\"}'\n  note: >-\n    Present and answering, but every path requires an API token issued by a journal editor. No\n    public token-request path is documented. The contract itself is PKP's, not the university's.\n- surface: api.uniandes.edu.co\n  operator: institution\n  status: 403\n  note: >-\n    Cloudflare WAF (\"Attention Required!\") on every path tried, including /, /docs, /swagger,\n    /openapi.json, /api-docs, /health, /v1 and /.well-known/openapi. The host exists under the\n    institution's own domain\
  \ and is protected rather than unconfigured, but nothing about what it\n    serves is publicly discoverable.\n- surface: repositorio.uniandes.edu.co (DSpace 7 \"Seneca\")\n  operator: institution\n  status: 403\n  note: >-\n    Bot-detection interstitial. A request to /oai/request or /server/api 302s to /challenge and\n    then answers 403 with a \"Bot Detection\" body, under a browser User-Agent as well as curl's.\n    Live and defended, not dead.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-los-andes-colombia/refs/heads/main/authentication/university-of-los-andes-colombia-authentication.yml
summary_line: openIdConnect/saml2/none · 3 schemes
tags:
- University
- Higher Education
- Education
- Colombia
- Latin America
- Private Research University
- Open Access
- Institutional Repository
- Research Data
- Scholarly Publishing
- OAI-PMH
- Identity Federation
- Library
- Research
---
