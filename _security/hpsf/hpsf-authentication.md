---
anonymous_access: true
api_key_in: []
auth_types:
- none
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Hpsf Authentication
name_suffix: Authentication
oauth_flows: []
overview: High Performance Software Foundation secures its APIs with none and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: High Performance Software Foundation
provider_slug: hpsf
scheme_count: 2
schemes:
- applies_to:
  - GET https://hpsf.io/wp-json/
  - GET https://hpsf.io/wp-json/tribe/events/v1/events
  - GET https://hpsf.io/wp-json/tribe/events/v1/venues
  - GET https://hpsf.io/wp-json/tribe/events/v1/organizers
  - GET https://hpsf.io/wp-json/tribe/events/v1/categories
  - GET https://hpsf.io/wp-json/tribe/events/v1/tags
  - GET https://hpsf.io/wp-json/tribe/events/v1/doc
  - GET https://hpsf.io/wp-json/tec/v1/docs
  name: Anonymous
  note: No credential of any kind is required to read the events surface or either contract. Verified with unauthenticated GETs returning HTTP 200 on 2026-09-13.
  type: none
- applies_to: All POST/PUT/PATCH/DELETE operations across tribe/events/v1 and tec/v1.
  authorization_endpoint: https://hpsf.io/wp-admin/authorize-application.php
  authorization_endpoint_source: Declared by the host itself in the authentication block of https://hpsf.io/wp-json/
  declared_in: openapi/hpsf-tec-events-api-openapi.yml
  header: 'Authorization: Basic <base64 username:application-password>'
  mechanism: WordPress Application Passwords
  name: BasicAuth
  note: Application Passwords are issued from inside the WordPress admin to an existing site user. HPSF publishes no process for a third party to obtain one, so the write half of both contracts is documented but unreachable from outside the foundation's own web team.
  public_onboarding: false
  scheme: basic
  type: http
slug: hpsf-authentication
source_filename: hpsf-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: searched\nsource: >-\n  https://hpsf.io/wp-json/ (the route index, which declares the Application Passwords authorization\n  endpoint), the BasicAuth securityScheme in the tec/v1 contract at https://hpsf.io/wp-json/tec/v1/docs,\n  and live anonymous calls against every namespace on 2026-09-13.\nname: HPSF authentication\nsummary:\n  types:\n  - none\n  - http\n  anonymous_read: true\n  api_keys: false\n  oauth2: false\n  oidc: false\n  mtls: false\nschemes:\n- name: Anonymous\n  type: none\n  applies_to:\n  - GET https://hpsf.io/wp-json/\n  - GET https://hpsf.io/wp-json/tribe/events/v1/events\n  - GET https://hpsf.io/wp-json/tribe/events/v1/venues\n  - GET https://hpsf.io/wp-json/tribe/events/v1/organizers\n  - GET https://hpsf.io/wp-json/tribe/events/v1/categories\n  - GET https://hpsf.io/wp-json/tribe/events/v1/tags\n  - GET https://hpsf.io/wp-json/tribe/events/v1/doc\n  - GET https://hpsf.io/wp-json/tec/v1/docs\n  note: >-\n    No credential\
  \ of any kind is required to read the events surface or either contract. Verified with\n    unauthenticated GETs returning HTTP 200 on 2026-09-13.\n- name: BasicAuth\n  type: http\n  scheme: basic\n  header: 'Authorization: Basic <base64 username:application-password>'\n  declared_in: openapi/hpsf-tec-events-api-openapi.yml\n  mechanism: WordPress Application Passwords\n  authorization_endpoint: https://hpsf.io/wp-admin/authorize-application.php\n  authorization_endpoint_source: >-\n    Declared by the host itself in the authentication block of https://hpsf.io/wp-json/\n  applies_to: All POST/PUT/PATCH/DELETE operations across tribe/events/v1 and tec/v1.\n  public_onboarding: false\n  note: >-\n    Application Passwords are issued from inside the WordPress admin to an existing site user. HPSF\n    publishes no process for a third party to obtain one, so the write half of both contracts is\n    documented but unreachable from outside the foundation's own web team.\ngated_surfaces:\n- namespace:\
  \ wp-abilities/v1\n  status: 401\n  code: rest_forbidden\n  note: >-\n    The WordPress Abilities registry is installed and registered on this host. An anonymous GET of\n    /wp-json/wp-abilities/v1/abilities returns 401 - the ability list, which is the closest thing this\n    host has to a machine-callable tool catalog, requires an authenticated WordPress user.\n- namespace: tec/v1\n  status: 400\n  code: missing_experimental_endpoint_acknowledgement\n  note: >-\n    Not an authentication gate. The namespace is fenced behind an undocumented acknowledgement header\n    for experimental endpoints, and rejects anonymous callers before any credential is considered.\n- namespaces: [activity-log/v1, objectcache/v1, liquidweb/harbor/v1, regenerate-thumbnails/v1, wp-site-health/v1, tec/v2/onboarding, tribe/event-aggregator/v1, tribe/zapier/v1, tribe/power-automate/v1]\n  note: >-\n    Site-administration and integration plugin routes, all permission-gated to a logged-in WordPress\n    administrator.\
  \ Present in the route index; not a public API surface.\nabsent:\n  api_key_header: null\n  oauth_scopes: null\n  note: >-\n    scopes/ is deliberately not written. There is no oauth2 securityScheme in either contract and no\n    OAuth documented anywhere, so an OAuthScopes artifact would be an empty claim.\nevidence:\n- url: https://hpsf.io/wp-json/tribe/events/v1/events?per_page=1\n  status: 200\n  note: Anonymous read succeeded with no credential.\n- url: https://hpsf.io/wp-json/\n  status: 200\n  note: 'authentication block names application-passwords with its authorization endpoint.'\n- url: https://hpsf.io/wp-json/wp-abilities/v1/abilities\n  status: 401\n- url: https://hpsf.io/.well-known/oauth-authorization-server\n  status: 404\n- url: https://hpsf.io/.well-known/openid-configuration\n  status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hpsf/refs/heads/main/authentication/hpsf-authentication.yml
summary_line: none/http · 2 schemes
tags:
- HPC
- Linux Foundation
- Open Source
- Scientific Computing
- Foundations
- Supercomputing
- Open Governance
- Event
- Conferences
- Research Computing
- Non-Profit
- Content
---
