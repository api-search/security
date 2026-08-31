---
api_key_in: []
api_specs:
- filename: university-of-warwick-administration-api-openapi.yml
  format: yaml
  label: University of Warwick Administration API
  slug: university-of-warwick-administration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-warwick/refs/heads/main/openapi/university-of-warwick-administration-api-openapi.yml
- filename: university-of-warwick-jobs-api-openapi.yml
  format: yaml
  label: University of Warwick Jobs API
  slug: university-of-warwick-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-warwick/refs/heads/main/openapi/university-of-warwick-jobs-api-openapi.yml
- filename: university-of-warwick-oai-pmh-api-openapi.yml
  format: yaml
  label: University of Warwick OAI PMH API
  slug: university-of-warwick-oai-pmh-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-warwick/refs/heads/main/openapi/university-of-warwick-oai-pmh-api-openapi.yml
- filename: university-of-warwick-timetabling-api-openapi.yml
  format: yaml
  label: University of Warwick Timetabling API
  slug: university-of-warwick-timetabling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-warwick/refs/heads/main/openapi/university-of-warwick-timetabling-api-openapi.yml
auth_types:
- http
- oauth1
- saml
description: ''
kind: authentication
layout: security
method: searched
name: University Of Warwick Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Warwick secures its APIs with http, oauth1, and saml across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: University of Warwick
provider_slug: university-of-warwick
scheme_count: 3
schemes:
- applies_to:
  - Tabula API (tabula.warwick.ac.uk/api)
  description: HTTP Basic authentication over HTTPS against Warwick Web Sign-on, using an ITS user code and password. Warwick documents that API requests SHOULD use a dedicated External User account provisioned for API access via the ITS web team, not a personal staff or student account.
  evidence: Probed https://tabula.warwick.ac.uk/api/v1/department unauthenticated on 2026-08-19 — HTTP 401, body {"success":false,"status":"unauthorized","errors":[{"message":"API requests must be authenticated with HTTP Basic Auth or OAuth"}]}.
  name: basicAuth
  scheme: basic
  sources:
  - https://warwick.ac.uk/services/idg/services-support/web/tabula/api/authentication
  type: http
- applies_to:
  - Tabula API
  - Sitebuilder
  - Warwick Search
  - Files.Warwick
  - Warwick Blogs
  - Warwick Forums
  - Exam Timetabling
  - Printer Credits
  - Web Sign-on
  description: Three-legged OAuth 1.0a issued by Warwick Web Sign-on. Request tokens are valid for five minutes. Applications must be registered with the ITS Web Team before a token will be issued. A Warwick-specific `scope` parameter — not part of the OAuth standard — names the service being accessed, and multiple scopes are joined with `+` in a single parameter.
  endpoints:
    access_token: https://websignon.warwick.ac.uk/oauth/accessToken
    authorize: https://websignon.warwick.ac.uk/oauth/authorise
    request_token: https://websignon.warwick.ac.uk/oauth/requestToken
  name: oauth1
  parameter_locations:
  - Authorization header (the `scope` parameter cannot be sent here)
  - query string
  - POST body
  scopes_artifact: scopes/university-of-warwick-oauth-scopes.yml
  signature_algorithms:
  - RSA-SHA1
  - HMAC-SHA1
  signature_note: RSA-SHA1 requires uploading a certificate at registration. HMAC-SHA1 requires no certificate; Warwick generates and issues the consumer secret after registration.
  sources:
  - https://warwick.ac.uk/services/its/servicessupport/web/sign-on/help/oauth/apis/
  type: oauth1
  version: 1.0a
- description: Warwick operates a Shibboleth identity provider as a member of the UK Access Management Federation and, through it, eduGAIN. The SAML 2.0 metadata is published unauthenticated and is machine-readable.
  entity_attributes:
    assurance_certification: https://refeds.org/sirtfi
    entity_category_support: http://refeds.org/category/research-and-scholarship
  entity_id: https://idp.warwick.ac.uk/idp/shibboleth
  evidence: Probed https://idp.warwick.ac.uk/idp/shibboleth on 2026-08-19 — HTTP 200, application/xml, 7,843 bytes, root element <EntityDescriptor> with entityID="https://idp.warwick.ac.uk/idp/shibboleth" and an IDPSSODescriptor.
  metadata_url: https://idp.warwick.ac.uk/idp/shibboleth
  name: shibboleth-saml
  protocols_supported:
  - urn:mace:shibboleth:1.0
  - urn:oasis:names:tc:SAML:1.1:protocol
  - urn:oasis:names:tc:SAML:2.0:protocol
  scope: warwick.ac.uk
  sources:
  - https://idp.warwick.ac.uk/idp/shibboleth
  type: saml
  version: SAML 2.0
slug: university-of-warwick-authentication
source_filename: university-of-warwick-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: searched\nsource: https://warwick.ac.uk/services/its/servicessupport/web/sign-on/help/oauth/apis/\ndocs: https://warwick.ac.uk/services/idg/services-support/web/tabula/api/authentication\nx-operator: institution\nnote: >-\n  Warwick operates its own central identity infrastructure — Web Sign-on (websignon.warwick.ac.uk)\n  and a Shibboleth SAML 2.0 identity provider (idp.warwick.ac.uk) — rather than delegating\n  authentication to a vendor platform. This is one of the few places where a university genuinely\n  IS the operator, and it is the most substantive part of Warwick's programmable surface.\n\n\n  Notable: Warwick still uses OAuth 1.0a, not OAuth 2.0, and there is no OpenID Connect discovery\n  document — https://warwick.ac.uk/.well-known/openid-configuration returns 404 (probed\n  2026-08-19). The OAuth surface is documented in prose only; no machine-readable discovery\n  document of any kind is published for it.\nsummary:\n  types: [http,\
  \ oauth1, saml]\n  oauth2: false\n  oidc: false\n  oidc_discovery_document: false\n  mtls: false\nschemes:\n  - name: basicAuth\n    type: http\n    scheme: basic\n    description: >-\n      HTTP Basic authentication over HTTPS against Warwick Web Sign-on, using an ITS user code\n      and password. Warwick documents that API requests SHOULD use a dedicated External User\n      account provisioned for API access via the ITS web team, not a personal staff or student\n      account.\n    applies_to:\n      - Tabula API (tabula.warwick.ac.uk/api)\n    sources:\n      - https://warwick.ac.uk/services/idg/services-support/web/tabula/api/authentication\n    evidence: >-\n      Probed https://tabula.warwick.ac.uk/api/v1/department unauthenticated on 2026-08-19 —\n      HTTP 401, body {\"success\":false,\"status\":\"unauthorized\",\"errors\":[{\"message\":\"API requests\n      must be authenticated with HTTP Basic Auth or OAuth\"}]}.\n  - name: oauth1\n    type: oauth1\n    version: 1.0a\n   \
  \ description: >-\n      Three-legged OAuth 1.0a issued by Warwick Web Sign-on. Request tokens are valid for five\n      minutes. Applications must be registered with the ITS Web Team before a token will be\n      issued. A Warwick-specific `scope` parameter — not part of the OAuth standard — names the\n      service being accessed, and multiple scopes are joined with `+` in a single parameter.\n    signature_algorithms: [RSA-SHA1, HMAC-SHA1]\n    signature_note: >-\n      RSA-SHA1 requires uploading a certificate at registration. HMAC-SHA1 requires no\n      certificate; Warwick generates and issues the consumer secret after registration.\n    endpoints:\n      request_token: https://websignon.warwick.ac.uk/oauth/requestToken\n      authorize: https://websignon.warwick.ac.uk/oauth/authorise\n      access_token: https://websignon.warwick.ac.uk/oauth/accessToken\n    parameter_locations:\n      - Authorization header (the `scope` parameter cannot be sent here)\n      - query string\n  \
  \    - POST body\n    applies_to:\n      - Tabula API\n      - Sitebuilder\n      - Warwick Search\n      - Files.Warwick\n      - Warwick Blogs\n      - Warwick Forums\n      - Exam Timetabling\n      - Printer Credits\n      - Web Sign-on\n    sources:\n      - https://warwick.ac.uk/services/its/servicessupport/web/sign-on/help/oauth/apis/\n    scopes_artifact: scopes/university-of-warwick-oauth-scopes.yml\n  - name: shibboleth-saml\n    type: saml\n    version: SAML 2.0\n    description: >-\n      Warwick operates a Shibboleth identity provider as a member of the UK Access Management\n      Federation and, through it, eduGAIN. The SAML 2.0 metadata is published unauthenticated\n      and is machine-readable.\n    entity_id: https://idp.warwick.ac.uk/idp/shibboleth\n    metadata_url: https://idp.warwick.ac.uk/idp/shibboleth\n    scope: warwick.ac.uk\n    protocols_supported:\n      - urn:mace:shibboleth:1.0\n      - urn:oasis:names:tc:SAML:1.1:protocol\n      - urn:oasis:names:tc:SAML:2.0:protocol\n\
  \    entity_attributes:\n      assurance_certification: https://refeds.org/sirtfi\n      entity_category_support: http://refeds.org/category/research-and-scholarship\n    evidence: >-\n      Probed https://idp.warwick.ac.uk/idp/shibboleth on 2026-08-19 — HTTP 200,\n      application/xml, 7,843 bytes, root element <EntityDescriptor> with\n      entityID=\"https://idp.warwick.ac.uk/idp/shibboleth\" and an IDPSSODescriptor.\n    sources:\n      - https://idp.warwick.ac.uk/idp/shibboleth\npublic_surface:\n  note: >-\n    Three Tabula calendar endpoints require no authentication at all and were verified returning\n    live data unauthenticated on 2026-08-19: /api/v1/termdates, /api/v1/termdates/weeks and\n    /api/v1/holidaydates, each also available as iCalendar. WRAP's OAI-PMH endpoint is likewise\n    fully open. Everything else on Warwick's surface is credentialed.\nx-evidence:\n  - url: https://tabula.warwick.ac.uk/api/v1/termdates\n    status: 200\n  - url: https://tabula.warwick.ac.uk/api/v1/department\n\
  \    status: 401\n  - url: https://idp.warwick.ac.uk/idp/shibboleth\n    status: 200\n  - url: https://warwick.ac.uk/.well-known/openid-configuration\n    status: 404\n  - url: https://warwick.ac.uk/services/its/servicessupport/web/sign-on/help/oauth/apis/\n    status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-warwick/refs/heads/main/authentication/university-of-warwick-authentication.yml
summary_line: http/oauth1/saml · 3 schemes
tags:
- University
- Higher Education
- Education
- Research
- United Kingdom
- Russell Group
- Identity Federation
- Research Repository
- Course Catalog
- Timetabling
- Student Information System
- Open Data
---
