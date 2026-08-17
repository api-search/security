---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Popmenu Authentication
name_suffix: Authentication
oauth_flows: []
overview: Popmenu declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Popmenu
provider_slug: popmenu
scheme_count: 0
schemes: []
slug: popmenu-authentication
source_filename: popmenu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://api.popmenu.com/graphql (live unauthenticated probes, 2026-08-13)\ndocumented: false\ndocs: null\nnote: >-\n  NO AUTHENTICATION POINTER IS EMITTED IN apis.yml. Popmenu does not document\n  authentication anywhere on its public surface — there is no auth page, no key format, no\n  header name, no token endpoint, and no scope reference. This artifact records what the\n  live endpoint does when called without credentials, which is a real measurement, but it\n  is not the provider documenting authentication, and wiring a `type: Authentication`\n  pointer would credit Popmenu with an ergonomics check it has not earned.\n  derive-authentication.py produced no profile for this slug because there is no OpenAPI to\n  derive one from.\nschemes: []\nscheme_count: 0\noauth2: false\nopenid_connect: false\nmutual_tls: false\napi_key:\n  documented: false\n  header_name: unknown\n  prefix: unknown\nobserved_behaviour:\n  endpoint: https://api.popmenu.com/graphql\n\
  \  unauthenticated_request:\n    method: POST\n    body: '{\"query\":\"{__typename}\"}'\n  response:\n    http_status: 200\n    body: '{\"errors\":[{\"friendlyMessage\":\"Sorry, you are not authorized to perform that action- try signing back in\",\"message\":\"unauthorized\"}]}'\n  interpretation: >-\n    Authentication is enforced ahead of query parsing and validation — an introspection\n    query, a trivial `{__typename}` query and a query naming a nonexistent field all return\n    the identical `unauthorized` envelope. The phrase \"try signing back in\" points at a\n    session-cookie model serving Popmenu's own first-party apps; how a third-party partner\n    presents credentials is not stated publicly.\ndiscovery_probes:\n- url: https://api.popmenu.com/.well-known/openid-configuration\n  status: 404\n- url: https://api.popmenu.com/.well-known/oauth-authorization-server\n  status: 404\n- url: https://api.popmenu.com/.well-known/oauth-protected-resource\n  status: 404\n- url: https://my.popmenu.com/.well-known/openid-configuration\n\
  \  status: 404\n- url: https://my.popmenu.com/.well-known/oauth-authorization-server\n  status: 404\n- url: https://get.popmenu.com/.well-known/openid-configuration\n  status: 403\n  note: Cloudflare bot challenge — unknown, not absent.\naccess_model:\n  self_service: false\n  route: >-\n    https://get.popmenu.com/developer-api is a lead-capture form. Submitting it lands on\n    https://get.popmenu.com/success-api — \"Thank you for your interest in working with\n    Popmenu! We'll be reaching out to you soon.\" Credentials are issued through a sales /\n    partner conversation.\n  sandbox: not-published\n  scopes: not-published\ngaps:\n- No published credential type, header name, or key prefix.\n- No token endpoint, refresh flow, or expiry policy published.\n- No OAuth or OIDC discovery document on any host.\n- No scope or permission reference, so `scopes/` is deliberately not written (there is no\n  OAuth surface to derive one from).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/popmenu/refs/heads/main/authentication/popmenu-authentication.yml
summary_line: 0 schemes
tags:
- Restaurant
- Menus
- Online Ordering
- Websites
- Marketing
- Integrations
- Hospitality
- GraphQL
- Point Of Sale
- Reservations
- Loyalty
- AI Marketing
---
