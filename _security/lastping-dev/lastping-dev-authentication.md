---
anonymous_access: false
api_key_in:
- cookie
- header
api_specs:
- filename: lastping-dev-agents-api-openapi.yml
  format: yaml
  label: LastPing Agents API
  slug: lastping-dev-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lastping-dev/openapi/lastping-dev-agents-api-openapi.yml
- filename: lastping-dev-auth-api-openapi.yml
  format: yaml
  label: LastPing Auth API
  slug: lastping-dev-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lastping-dev/openapi/lastping-dev-auth-api-openapi.yml
- filename: lastping-dev-channels-api-openapi.yml
  format: yaml
  label: LastPing Channels API
  slug: lastping-dev-channels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lastping-dev/openapi/lastping-dev-channels-api-openapi.yml
- filename: lastping-dev-checks-api-openapi.yml
  format: yaml
  label: LastPing Checks API
  slug: lastping-dev-checks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lastping-dev/openapi/lastping-dev-checks-api-openapi.yml
- filename: lastping-dev-ci-api-openapi.yml
  format: yaml
  label: LastPing CI API
  slug: lastping-dev-ci-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lastping-dev/openapi/lastping-dev-ci-api-openapi.yml
- filename: lastping-dev-discovery-api-openapi.yml
  format: yaml
  label: LastPing Discovery API
  slug: lastping-dev-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lastping-dev/openapi/lastping-dev-discovery-api-openapi.yml
- filename: lastping-dev-events-api-openapi.yml
  format: yaml
  label: LastPing Events API
  slug: lastping-dev-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lastping-dev/openapi/lastping-dev-events-api-openapi.yml
- filename: lastping-dev-export-api-openapi.yml
  format: yaml
  label: LastPing Export API
  slug: lastping-dev-export-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lastping-dev/openapi/lastping-dev-export-api-openapi.yml
- filename: lastping-dev-health-api-openapi.yml
  format: yaml
  label: LastPing Health API
  slug: lastping-dev-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lastping-dev/openapi/lastping-dev-health-api-openapi.yml
- filename: lastping-dev-incidents-api-openapi.yml
  format: yaml
  label: LastPing Incidents API
  slug: lastping-dev-incidents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lastping-dev/openapi/lastping-dev-incidents-api-openapi.yml
- filename: lastping-dev-metrics-api-openapi.yml
  format: yaml
  label: LastPing Metrics API
  slug: lastping-dev-metrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lastping-dev/openapi/lastping-dev-metrics-api-openapi.yml
- filename: lastping-dev-monitors-api-openapi.yml
  format: yaml
  label: LastPing Monitors API
  slug: lastping-dev-monitors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lastping-dev/openapi/lastping-dev-monitors-api-openapi.yml
- filename: lastping-dev-routes-api-openapi.yml
  format: yaml
  label: LastPing Routes API
  slug: lastping-dev-routes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lastping-dev/openapi/lastping-dev-routes-api-openapi.yml
- filename: lastping-dev-statuspages-api-openapi.yml
  format: yaml
  label: LastPing Status Pages API
  slug: lastping-dev-statuspages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lastping-dev/openapi/lastping-dev-statuspages-api-openapi.yml
- filename: lastping-dev-traces-api-openapi.yml
  format: yaml
  label: LastPing Traces API
  slug: lastping-dev-traces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lastping-dev/openapi/lastping-dev-traces-api-openapi.yml
- filename: lastping-dev-api-keys-api-openapi.yml
  format: yaml
  label: LastPing API Keys API
  slug: lastping-dev-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lastping-dev/openapi/lastping-dev-api-keys-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: derived
name: LastPing Authentication
name_suffix: Authentication
oauth_flows: []
overview: LastPing secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: LastPing
provider_slug: lastping-dev
scheme_count: 3
schemes:
- description: 'Project API key.  Obtain from your LastPing project settings.


    **Every key carries a scope**, which is what it is permitted to do:


    | Scope | Reaches |

    | --- | --- |

    | `read` | Every `GET`. |

    | `write` | Everything except API key management — the default for a new key. |

    | `admin` | Everything, including `/api/v1/api-keys`. |


    A request whose key ranks below an operation''s requirement is refused

    w'
  in: header
  name: ApiKeyAuth
  parameter: X-Api-Key
  sources:
  - openapi/lastping-dev-openapi.yaml
  type: apiKey
- description: 'Project API key presented as a Bearer token.

    Accepted as an alternative to the X-Api-Key header, specifically

    to allow Prometheus scrape_config `authorization: { credentials: … }`.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/lastping-dev-openapi.yaml
  type: http
- description: 'The signed-in browser session, set by the sign-in flow at

    `/auth/login`. It is `HttpOnly`, `Secure` and `SameSite=Lax`, so it

    cannot be read by script and is not a credential you can obtain or

    store the way an API key is.


    A handful of operations accept **only** this, and refuse an API key of

    any scope with `403 SESSION_ONLY`. They act on a PERSON rather than on a

    project (`/api/v1/me/password`, `'
  in: cookie
  name: SessionCookie
  parameter: lp_session
  sources:
  - openapi/lastping-dev-openapi.yaml
  type: apiKey
slug: lastping-dev-authentication
source_filename: lastping-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: derived\nsource: openapi/lastping-dev-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: |-\n    Project API key.  Obtain from your LastPing project settings.\n\n    **Every key carries a scope**, which is what it is permitted to do:\n\n    | Scope | Reaches |\n    | --- | --- |\n    | `read` | Every `GET`. |\n    | `write` | Everything except API key management — the default for a new key. |\n    | `admin` | Everything, including `/api/v1/api-keys`. |\n\n    A request whose key ranks below an operation's requirement is refused\n    w\n  sources:\n  - openapi/lastping-dev-openapi.yaml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: |-\n    Project API key presented as a Bearer token.\n    Accepted as an alternative to the X-Api-Key header, specifically\n    to allow Prometheus scrape_config\
  \ `authorization: { credentials: … }`.\n  sources:\n  - openapi/lastping-dev-openapi.yaml\n- name: SessionCookie\n  type: apiKey\n  in: cookie\n  parameter: lp_session\n  description: |-\n    The signed-in browser session, set by the sign-in flow at\n    `/auth/login`. It is `HttpOnly`, `Secure` and `SameSite=Lax`, so it\n    cannot be read by script and is not a credential you can obtain or\n    store the way an API key is.\n\n    A handful of operations accept **only** this, and refuse an API key of\n    any scope with `403 SESSION_ONLY`. They act on a PERSON rather than on a\n    project (`/api/v1/me/password`, `\n  sources:\n  - openapi/lastping-dev-openapi.yaml\n"
source_yaml_url: https://artifacts.apis.io/lastping-dev/authentication/lastping-dev-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Monitoring
- Artificial Intelligence
- DevOps
- Open Source
- Automation
---
