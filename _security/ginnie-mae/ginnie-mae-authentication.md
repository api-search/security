---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ginnie-mae-block-content-api-openapi.yml
  format: yaml
  label: Ginnie Mae Block Content API
  slug: ginnie-mae-block-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ginnie-mae/refs/heads/main/openapi/ginnie-mae-block-content-api-openapi.yml
- filename: ginnie-mae-disclosure-api-openapi.yml
  format: yaml
  label: Ginnie Mae Disclosure API
  slug: ginnie-mae-disclosure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ginnie-mae/refs/heads/main/openapi/ginnie-mae-disclosure-api-openapi.yml
- filename: ginnie-mae-discovery-api-openapi.yml
  format: yaml
  label: Ginnie Mae Discovery API
  slug: ginnie-mae-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ginnie-mae/refs/heads/main/openapi/ginnie-mae-discovery-api-openapi.yml
- filename: ginnie-mae-entity-subqueue-api-openapi.yml
  format: yaml
  label: Ginnie Mae Entity Subqueue API
  slug: ginnie-mae-entity-subqueue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ginnie-mae/refs/heads/main/openapi/ginnie-mae-entity-subqueue-api-openapi.yml
- filename: ginnie-mae-faq-api-openapi.yml
  format: yaml
  label: Ginnie Mae FAQ API
  slug: ginnie-mae-faq-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ginnie-mae/refs/heads/main/openapi/ginnie-mae-faq-api-openapi.yml
- filename: ginnie-mae-file-api-openapi.yml
  format: yaml
  label: Ginnie Mae File API
  slug: ginnie-mae-file-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ginnie-mae/refs/heads/main/openapi/ginnie-mae-file-api-openapi.yml
- filename: ginnie-mae-media-api-openapi.yml
  format: yaml
  label: Ginnie Mae Media API
  slug: ginnie-mae-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ginnie-mae/refs/heads/main/openapi/ginnie-mae-media-api-openapi.yml
- filename: ginnie-mae-menu-api-openapi.yml
  format: yaml
  label: Ginnie Mae Menu API
  slug: ginnie-mae-menu-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ginnie-mae/refs/heads/main/openapi/ginnie-mae-menu-api-openapi.yml
- filename: ginnie-mae-menu-link-content-api-openapi.yml
  format: yaml
  label: Ginnie Mae Menu Link Content API
  slug: ginnie-mae-menu-link-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ginnie-mae/refs/heads/main/openapi/ginnie-mae-menu-link-content-api-openapi.yml
- filename: ginnie-mae-newsroom-api-openapi.yml
  format: yaml
  label: Ginnie Mae Newsroom API
  slug: ginnie-mae-newsroom-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ginnie-mae/refs/heads/main/openapi/ginnie-mae-newsroom-api-openapi.yml
- filename: ginnie-mae-node-api-openapi.yml
  format: yaml
  label: Ginnie Mae Node API
  slug: ginnie-mae-node-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ginnie-mae/refs/heads/main/openapi/ginnie-mae-node-api-openapi.yml
- filename: ginnie-mae-paragraph-api-openapi.yml
  format: yaml
  label: Ginnie Mae Paragraph API
  slug: ginnie-mae-paragraph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ginnie-mae/refs/heads/main/openapi/ginnie-mae-paragraph-api-openapi.yml
- filename: ginnie-mae-search-api-openapi.yml
  format: yaml
  label: Ginnie Mae Search API
  slug: ginnie-mae-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ginnie-mae/refs/heads/main/openapi/ginnie-mae-search-api-openapi.yml
- filename: ginnie-mae-site-content-api-openapi.yml
  format: yaml
  label: Ginnie Mae Site Content API
  slug: ginnie-mae-site-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ginnie-mae/refs/heads/main/openapi/ginnie-mae-site-content-api-openapi.yml
- filename: ginnie-mae-taxonomy-term-api-openapi.yml
  format: yaml
  label: Ginnie Mae Taxonomy Term API
  slug: ginnie-mae-taxonomy-term-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ginnie-mae/refs/heads/main/openapi/ginnie-mae-taxonomy-term-api-openapi.yml
auth_types: []
description: 'Authentication profile for Ginnie Mae''s public API surface. There is no credential to obtain and none is advertised: the JSON:API content surface answers anonymous requests in full. Everything Ginnie Mae does gate sits on different hosts and is not an API.'
kind: authentication
layout: security
mechanism_count: 0
method: probed
name: Ginnie Mae Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ginnie Mae declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Ginnie Mae
provider_slug: ginnie-mae
scheme_count: 0
schemes: []
slug: ginnie-mae-authentication
source_filename: ginnie-mae-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: >-\n  Live anonymous probes of https://www.ginniemae.gov/api/v1/ and the ginniemae.gov\n  authentication surfaces, 2026-09-12.\nprovider: Ginnie Mae\nproviderId: ginnie-mae\ndescription: >-\n  Authentication profile for Ginnie Mae's public API surface. There is no\n  credential to obtain and none is advertised: the JSON:API content surface answers\n  anonymous requests in full. Everything Ginnie Mae does gate sits on different\n  hosts and is not an API.\nschemes: []\nsummary:\n  requires_authentication: false\n  scheme_count: 0\n  note: >-\n    Every one of the 120 JSON:API resource collections at\n    https://www.ginniemae.gov/api/v1/ returned HTTP 200 to an unauthenticated GET\n    on 2026-09-12, as did all nine Views REST exports and the RFC 9264 linksets.\n    No Authorization header, API key, cookie or referer was sent. The OpenAPI in\n    openapi/ therefore declares no securitySchemes — an accurate description of the\n\
  \    surface, not a gap in the description.\napis:\n  - aid: ginnie-mae:ginnie-mae-content-api\n    baseURL: https://www.ginniemae.gov/api/v1\n    authentication: none\n    evidence: 'HTTP 200 anonymous on 120/120 collections, 2026-09-12'\ngated_surfaces:\n  - name: MyGinnieMae Enterprise Portal\n    host: my.ginniemae.gov\n    mechanism: SSO / partner login\n    evidence: >-\n      https://my.ginniemae.gov/webcenter/portal/public 302s to\n      https://access.ginniemae.gov/auth (Oracle Access Manager), HTTP 200 at the\n      login challenge. Issuer, document-custodian and pool-processing systems live\n      behind it. Probed 2026-09-12.\n  - name: Disclosure Data Download\n    host: bulk.ginniemae.gov\n    mechanism: free registered account (email + secret question + emailed key)\n    evidence: >-\n      https://bulk.ginniemae.gov/ HTTP 200 serves an Angular client whose runtime\n      configuration (https://bulk.ginniemae.gov/assets/config/config.prod.json,\n      HTTP 200) names a download\
  \ service at\n      https://www.ginniemae.gov/disclosure-api/api and a login route at\n      https://www.ginniemae.gov/disclosure/download-login. Anonymous GET of the\n      download service returns the SPA shell, not data. Account creation is at\n      https://www.ginniemae.gov/disclosure/create-account. Probed 2026-09-12.\n  - name: Subscription / user-profile services\n    host: www.ginniemae.gov\n    mechanism: account session\n    evidence: >-\n      https://www.ginniemae.gov/subscriptions/api and\n      https://www.ginniemae.gov/user-profiles/api both return HTTP 403 to an\n      anonymous request. Probed 2026-09-12.\noauth:\n  published: false\n  note: >-\n    Drupal's simple_oauth module is installed (consumer--consumer,\n    oauth2_scope--oauth2_scope and oauth2_token--access_token / auth_code /\n    refresh_token are all exposed as JSON:API resource types) but no authorization\n    server is published. /.well-known/oauth-authorization-server,\n    /.well-known/oauth-protected-resource,\
  \ /.well-known/openid-configuration and\n    /oauth/token each return HTTP 200 with the Angular application shell rather\n    than metadata — an SPA catch-all, not a document. No scopes/ artifact is written\n    for this provider because there is no scope surface to describe.\ndocs: null\ndocs_note: >-\n  Ginnie Mae publishes no authentication documentation for this API because it\n  publishes no documentation for the API at all.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ginnie-mae/refs/heads/main/authentication/ginnie-mae-authentication.yml
summary_line: 0 schemes
tags:
- Federal Government
- Housing
- Mortgage
- Mortgage-Backed Securities
- Open Data
- Content
- JSON:API
---
