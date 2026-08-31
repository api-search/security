---
api_key_in: []
api_specs:
- filename: alzheon-comments-api-openapi.yml
  format: yaml
  label: Alzheon Comments API
  slug: alzheon-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alzheon/refs/heads/main/openapi/alzheon-comments-api-openapi.yml
- filename: alzheon-discovery-api-openapi.yml
  format: yaml
  label: Alzheon Discovery API
  slug: alzheon-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alzheon/refs/heads/main/openapi/alzheon-discovery-api-openapi.yml
- filename: alzheon-faq-api-openapi.yml
  format: yaml
  label: Alzheon FAQ API
  slug: alzheon-faq-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alzheon/refs/heads/main/openapi/alzheon-faq-api-openapi.yml
- filename: alzheon-media-api-openapi.yml
  format: yaml
  label: Alzheon Media API
  slug: alzheon-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alzheon/refs/heads/main/openapi/alzheon-media-api-openapi.yml
- filename: alzheon-metadata-api-openapi.yml
  format: yaml
  label: Alzheon Metadata API
  slug: alzheon-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alzheon/refs/heads/main/openapi/alzheon-metadata-api-openapi.yml
- filename: alzheon-oembed-api-openapi.yml
  format: yaml
  label: Alzheon O Embed API
  slug: alzheon-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alzheon/refs/heads/main/openapi/alzheon-oembed-api-openapi.yml
- filename: alzheon-pages-api-openapi.yml
  format: yaml
  label: Alzheon Pages API
  slug: alzheon-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alzheon/refs/heads/main/openapi/alzheon-pages-api-openapi.yml
- filename: alzheon-portfolio-api-openapi.yml
  format: yaml
  label: Alzheon Portfolio API
  slug: alzheon-portfolio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alzheon/refs/heads/main/openapi/alzheon-portfolio-api-openapi.yml
- filename: alzheon-posts-api-openapi.yml
  format: yaml
  label: Alzheon Posts API
  slug: alzheon-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alzheon/refs/heads/main/openapi/alzheon-posts-api-openapi.yml
- filename: alzheon-search-api-openapi.yml
  format: yaml
  label: Alzheon Search API
  slug: alzheon-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alzheon/refs/heads/main/openapi/alzheon-search-api-openapi.yml
- filename: alzheon-taxonomy-api-openapi.yml
  format: yaml
  label: Alzheon Taxonomy API
  slug: alzheon-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alzheon/refs/heads/main/openapi/alzheon-taxonomy-api-openapi.yml
- filename: alzheon-users-api-openapi.yml
  format: yaml
  label: Alzheon Users API
  slug: alzheon-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alzheon/refs/heads/main/openapi/alzheon-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Alzheon Authentication
name_suffix: Authentication
oauth_flows: []
overview: Alzheon secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Alzheon
provider_slug: alzheon
scheme_count: 1
schemes:
- applies_to: write and administrative routes
  description: WordPress application passwords (HTTP Basic — WordPress username plus a generated application password). Advertised by the site's own route index under authentication.application-passwords, with the authorization endpoint at https://alzheon.com/wp-admin/authorize-application.php. Required only for write and administrative routes, none of which are in the OpenAPI. Alzheon issues no public credentials, so this scheme is declared but unreachable for third parties.
  name: applicationPassword
  reachable_by_third_parties: false
  rfc: RFC 7617
  scheme: basic
  sources:
  - openapi/alzheon-content-openapi.yml
  - https://alzheon.com/wp-json/
  type: http
slug: alzheon-authentication
source_filename: alzheon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: derived\nsource: >-\n  openapi/alzheon-content-openapi.yml, plus the authentication block of the live route index\n  at https://alzheon.com/wp-json/ and anonymous probes on 2026-07-31\nnote: >-\n  Alzheon publishes no authentication documentation — there was no docs page to search, so\n  this stays derived. The whole public surface is anonymous: no key is issued, no signup\n  exists, and the only declared scheme is closed in practice.\nsummary:\n  types:\n  - http\n  anonymous_read: true\n  credentials_issued_publicly: false\n  api_keys: false\n  oauth2: false\n  oidc: false\n  mtls: false\n  signup_url: null\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  rfc: RFC 7617\n  description: >-\n    WordPress application passwords (HTTP Basic — WordPress username plus a generated\n    application password). Advertised by the site's own route index under\n    authentication.application-passwords, with the authorization endpoint\
  \ at\n    https://alzheon.com/wp-admin/authorize-application.php. Required only for write and\n    administrative routes, none of which are in the OpenAPI. Alzheon issues no public\n    credentials, so this scheme is declared but unreachable for third parties.\n  applies_to: write and administrative routes\n  reachable_by_third_parties: false\n  sources:\n  - openapi/alzheon-content-openapi.yml\n  - https://alzheon.com/wp-json/\nanonymous_access:\n  applies_to: every operation in openapi/alzheon-content-openapi.yml\n  verified: '2026-07-31'\n  detail: >-\n    All read operations were probed without any credential and returned HTTP 200.\n    Administrative routes excluded from the spec return 401 with code rest_forbidden or\n    rest_cannot_view_plugins.\n  cors:\n    allow_headers: [Authorization, X-WP-Nonce, Content-Disposition, Content-MD5, Content-Type]\n    expose_headers: [X-WP-Total, X-WP-TotalPages, Link]\n    note: >-\n      X-WP-Nonce is the cookie-authenticated browser flow used\
  \ by the site's own admin\n      screens; it is not available to third-party clients.\nnot_present:\n- mechanism: api-key\n  evidence: no apiKey securityScheme; no key issuance or signup page exists\n- mechanism: oauth2\n  evidence: /.well-known/oauth-authorization-server and /.well-known/oauth-protected-resource both 404\n- mechanism: openIdConnect\n  evidence: /.well-known/openid-configuration returns 404\n- mechanism: mutualTLS\n  evidence: no mTLS requirement observed\n- mechanism: jwt\n  evidence: no JWT plugin namespace present in the route index\nsee_also:\n  scopes: null\n  conventions: conventions/alzheon-conventions.yml\n  domain_security: security/alzheon-domain-security.yml\n  well_known: well-known/alzheon-well-known.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alzheon/refs/heads/main/authentication/alzheon-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Life Sciences
- Clinical Trials
- Alzheimer's Disease
- Neurology
- Drug Development
- Healthcare
- Private Company
---
