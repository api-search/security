---
api_key_in: []
api_specs:
- filename: unsw-sydney-unsworks-dspace-openapi.yml
  format: yaml
  label: UNSWorks Repository REST API (DSpace 7.0)
  slug: unsworks-rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unsw-sydney/refs/heads/main/openapi/unsw-sydney-unsworks-dspace-openapi.yml
- filename: unsw-sydney-unsworks-oai-pmh-openapi.yml
  format: yaml
  label: UNSWorks Repository OAI-PMH
  slug: unsworks-oai
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unsw-sydney/refs/heads/main/openapi/unsw-sydney-unsworks-oai-pmh-openapi.yml
auth_types: []
description: How each UNSW surface authenticates, established by probing rather than by reading marketing copy. The institution's most substantial API platform is fully gated; its readable surfaces are anonymous; and its own identity plane is a federated SAML IdP rather than an API key system.
kind: authentication
layout: security
method: probed
name: Unsw Sydney Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of New South Wales declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: University of New South Wales
provider_slug: unsw-sydney
scheme_count: 0
schemes: []
slug: unsw-sydney-authentication
source_filename: unsw-sydney-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "---\nname: UNSW Sydney — authentication posture by surface\naid: unsw-sydney\ngenerated: '2026-08-19'\nmethod: probed\nsource:\n  - https://apideveloper.unsw.edu.au/getting-started\n  - https://apideveloper.unsw.edu.au/signin\n  - https://unsworks.unsw.edu.au/server/api\n  - https://unsworks.unsw.edu.au/server/api/core/items?size=1\n  - https://unsworks.unsw.edu.au/server/api/core/bitstreams?size=1\n  - https://unsworks.unsw.edu.au/oai/request?verb=Identify\n  - https://aaf.unsw.edu.au/idp/shibboleth\ndescription: >-\n  How each UNSW surface authenticates, established by probing rather than by reading marketing\n  copy. The institution's most substantial API platform is fully gated; its readable surfaces are\n  anonymous; and its own identity plane is a federated SAML IdP rather than an API key system.\nsurfaces:\n  - surface: UNSW Enterprise Developer Portal / Enterprise API Gateway\n    host: apideveloper.unsw.edu.au\n    x-operator: institution\n    scheme: gated — request-based\
  \ authorisation, then Azure API Management subscription keys\n    self_service_signup: false\n    evidence:\n      - url: https://apideveloper.unsw.edu.au/signin\n        status: 200\n        detail: Sign-in page only; there is no self-service registration path.\n      - url: https://apideveloper.unsw.edu.au/getting-started\n        status: 200\n        detail: >-\n          The portal's own onboarding text states that consumers must complete a registration form\n          and may need to supply \"a DSA or approval from an authorised personnel\"; that credentials\n          are issued by the integration team; and explicitly that \"you will not be able to try out\n          the APIs in the Developer Portal, due to security constraints of the organisation.\"\n          Separate production-credential request forms exist for providers and consumers.\n      - url: https://apideveloper.unsw.edu.au/apis\n        status: 404\n        detail: No public API catalogue is exposed; the catalogue is\
  \ visible only after sign-in.\n    notes: >-\n      No base URL for the gateway itself is publicly disclosed anywhere on the portal. The\n      apideveloper hostname and api.unsw.edu.au share an IP (20.248.141.24); api.unsw.edu.au\n      itself returns 502 to unauthenticated requests and is not a documented public surface.\n  - surface: UNSWorks Repository REST API (DSpace 7.0)\n    host: unsworks.unsw.edu.au\n    x-operator: institution\n    scheme: anonymous read for discovery; session/JWT required for object browse endpoints\n    self_service_signup: n/a\n    evidence:\n      - url: https://unsworks.unsw.edu.au/server/api\n        status: 200\n        detail: Service document readable with no credentials.\n      - url: https://unsworks.unsw.edu.au/server/api/discover/search/objects?size=1\n        status: 200\n        detail: Discovery search readable with no credentials — the practical public entry point.\n      - url: https://unsworks.unsw.edu.au/server/api/core/communities?size=2\n\
  \        status: 200\n      - url: https://unsworks.unsw.edu.au/server/api/core/collections?size=1\n        status: 200\n      - url: https://unsworks.unsw.edu.au/server/api/core/items?size=1\n        status: 401\n        detail: >-\n          Unbounded item browse is gated. This is an access-clarity finding, not a failure: the\n          repository is publicly harvestable via discovery search and OAI-PMH, but the item\n          browse endpoint is not open.\n      - url: https://unsworks.unsw.edu.au/server/api/core/bitstreams?size=1\n        status: 401\n    notes: >-\n      DSpace exposes an authn endpoint at /server/api/authn; no credential issuance process for\n      external developers is documented publicly.\n  - surface: UNSWorks OAI-PMH\n    host: unsworks.unsw.edu.au\n    x-operator: institution\n    scheme: none — fully anonymous\n    evidence:\n      - url: https://unsworks.unsw.edu.au/oai/request?verb=Identify\n        status: 200\n        detail: All six OAI-PMH verbs answered\
  \ anonymously; no key, token or referrer required.\n  - surface: UNSW Shibboleth Identity Provider (AAF / eduGAIN)\n    host: aaf.unsw.edu.au\n    x-operator: institution\n    scheme: SAML 2.0 federated single sign-on (Shibboleth IdP)\n    evidence:\n      - url: https://aaf.unsw.edu.au/idp/shibboleth\n        status: 200\n        detail: >-\n          Entity metadata is served anonymously and is itself the machine-readable contract.\n          SSO endpoints require a valid SAML AuthnRequest from a federated service provider;\n          they are not an open API and were not exercised.\n    notes: >-\n      This is the institution's own identity plane and the reason a university's most reliable\n      programmable surface is often federation metadata rather than a REST API.\n  - surface: Moodle @ UNSW (TELT) LTI 1.3 platform\n    host: moodle.telt.unsw.edu.au\n    x-operator: tenant\n    scheme: OAuth 2.0 client credentials over LTI 1.3 (JWKS-published RS256 keys)\n    evidence:\n     \
  \ - url: https://moodle.telt.unsw.edu.au/mod/lti/certs.php\n        status: 200\n        detail: Public keyset served anonymously.\n      - url: https://moodle.telt.unsw.edu.au/mod/lti/token.php\n        status: 400\n        detail: Token endpoint present; rejects a request with no grant, which confirms it is live.\n      - url: https://moodle.telt.unsw.edu.au/webservice/rest/server.php\n        status: 200\n        detail: >-\n          Moodle web-service endpoint returns an in-band invalidtoken exception; token issuance is\n          internal to UNSW and not available to external developers.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unsw-sydney/refs/heads/main/authentication/unsw-sydney-authentication.yml
summary_line: 0 schemes
tags:
- University
- Higher Education
- Education
- Research
- Australia
- Group of Eight
- Sydney
- Research Repository
- Identity Federation
- Course Catalog
- Library
- Open Repository
---
