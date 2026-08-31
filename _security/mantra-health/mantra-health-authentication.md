---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Mantra Health Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mantra Health declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Mantra Health
provider_slug: mantra-health
scheme_count: 1
schemes:
- id: unknown-bearer-or-session
  in: unknown
  note: The credential type could not be established. The GraphQL endpoint accepts anonymous POSTs and returns a well-formed GraphQL response for the meta field {__typename} (-> "Query") without any credential, so it does not challenge unauthenticated callers at the transport layer. It returns no WWW-Authenticate header. Every non-meta query is rejected before execution with a generic validation error, so no authenticated field was ever reached and no auth mechanism was exercised.
  observed: false
  type: unknown
slug: mantra-health-authentication
source_filename: mantra-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: https://api.mantrahealth.com/graphql\nname: Mantra Health API authentication\nnote: >-\n  DERIVATION WAS NOT POSSIBLE and nothing has been invented. There is no OpenAPI to read\n  securitySchemes from, GraphQL introspection is disabled, and Mantra publishes no authentication\n  documentation because it publishes no developer portal at all. Everything below is what live\n  anonymous probes actually observed on 2026-08-25.\ndocumented: false\ndocs: null\ndocs_note: >-\n  No auth page exists. Mantra Health has no developer portal, API reference, getting-started guide or\n  public API documentation on any host; the site's own page-sitemap.xml lists no developer page.\nschemes:\n- id: unknown-bearer-or-session\n  type: unknown\n  in: unknown\n  observed: false\n  note: >-\n    The credential type could not be established. The GraphQL endpoint accepts anonymous POSTs and\n    returns a well-formed GraphQL response for the meta field\
  \ {__typename} (-> \"Query\") without any\n    credential, so it does not challenge unauthenticated callers at the transport layer. It returns\n    no WWW-Authenticate header. Every non-meta query is rejected before execution with a generic\n    validation error, so no authenticated field was ever reached and no auth mechanism was exercised.\nobserved_behaviour:\n  anonymous_reachable: true\n  anonymous_reachable_note: >-\n    POST https://api.mantrahealth.com/graphql with Content-Type application/json and\n    {\"query\":\"{__typename}\"} returns HTTP 200 {\"data\":{\"__typename\":\"Query\"}}.\n  www_authenticate_header: not_present\n  introspection: disabled\n  introspection_note: >-\n    A full introspection query and any unknown field both return HTTP 400\n    {\"errors\":[{\"message\":\"Invalid request.\",\"extensions\":{\"code\":\"GRAPHQL_VALIDATION_FAILED\"}}]}.\n    The response is identical for a syntactically valid introspection query and for a nonsense field,\n    so the server\
  \ is not merely hiding the schema — it appears to reject any operation outside an\n    allowed set. Consistent with an Apollo persisted-query / operation-safelist posture, but Mantra\n    documents nothing, so this is recorded as an observation, not a conclusion.\n  csrf_prevention: true\n  csrf_prevention_note: >-\n    Apollo Server CSRF prevention is enabled. A GET or a request without a JSON content-type returns\n    HTTP 400 with \"This operation has been blocked as a potential Cross-Site Request Forgery (CSRF).\n    Please either specify a 'content-type' header ... or provide a non-empty value for one of the\n    following headers: x-apollo-operation-name, apollo-require-preflight\".\n  cors_credentials: true\n  cors_credentials_note: >-\n    Response carries access-control-allow-credentials true, implying cookie/session-based browser auth\n    for the first-party portals.\nsso:\n  present: true\n  evidence:\n    url: https://mantrahealth.statuspage.io/api/v2/summary.json\n    http_status:\
  \ 200\n    quote: The status page lists an \"SSO\" component (operational).\n  protocol: unknown\n  note: >-\n    Campus single sign-on is operationally real — it has its own status component — but the protocol\n    is not published, and no OIDC or OAuth discovery document is served on any Mantra host. SAML is\n    the common choice in higher education; it is NOT asserted here because nothing observed confirms it.\ndiscovery_documents_probed:\n- url: https://api.mantrahealth.com/.well-known/openid-configuration\n  status: 404\n- url: https://api.mantrahealth.com/.well-known/oauth-authorization-server\n  status: 404\n- url: https://api.mantrahealth.com/.well-known/oauth-protected-resource\n  status: 404\n- url: https://mantrahealth.com/.well-known/openid-configuration\n  status: 301\n  note: Redirects to the homepage (soft-404).\nscopes:\n  present: unknown\n  note: >-\n    No scopes artifact is emitted. scopes/ is OAuth-only, and no OAuth 2.0 surface could be confirmed;\n    forcing an\
  \ empty scope list would assert a model that has not been observed.\nevidence:\n- url: https://api.mantrahealth.com/graphql\n  status: 200\n  note: Anonymous {__typename} succeeds.\n- url: https://api.mantrahealth.com/graphql\n  status: 400\n  note: Introspection and unknown fields rejected with GRAPHQL_VALIDATION_FAILED.\n- url: https://api.mantrahealth.com/\n  status: 200\n  note: Plain-text banner \"Mantra Health API\".\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mantra-health/refs/heads/main/authentication/mantra-health-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Healthcare
- Mental Health
- Telehealth
- Higher Education
- Digital Health
- Patient Engagement
- HIPAA
- GraphQL
---
