---
anonymous_access: false
api_key_in: []
api_specs:
- filename: automotive-grade-linux-categories-api-openapi.yml
  format: yaml
  label: Automotive Grade Linux Categories API
  slug: automotive-grade-linux-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automotive-grade-linux/refs/heads/main/openapi/automotive-grade-linux-categories-api-openapi.yml
- filename: automotive-grade-linux-common-api-openapi.yml
  format: yaml
  label: Automotive Grade Linux Common API
  slug: automotive-grade-linux-common-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automotive-grade-linux/refs/heads/main/openapi/automotive-grade-linux-common-api-openapi.yml
- filename: automotive-grade-linux-doc-api-openapi.yml
  format: yaml
  label: Automotive Grade Linux Doc API
  slug: automotive-grade-linux-doc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automotive-grade-linux/refs/heads/main/openapi/automotive-grade-linux-doc-api-openapi.yml
- filename: automotive-grade-linux-events-api-openapi.yml
  format: yaml
  label: Automotive Grade Linux Events API
  slug: automotive-grade-linux-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automotive-grade-linux/refs/heads/main/openapi/automotive-grade-linux-events-api-openapi.yml
- filename: automotive-grade-linux-events-pro-api-openapi.yml
  format: yaml
  label: Automotive Grade Linux Events Pro API
  slug: automotive-grade-linux-events-pro-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automotive-grade-linux/refs/heads/main/openapi/automotive-grade-linux-events-pro-api-openapi.yml
- filename: automotive-grade-linux-organizers-api-openapi.yml
  format: yaml
  label: Automotive Grade Linux Organizers API
  slug: automotive-grade-linux-organizers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automotive-grade-linux/refs/heads/main/openapi/automotive-grade-linux-organizers-api-openapi.yml
- filename: automotive-grade-linux-tags-api-openapi.yml
  format: yaml
  label: Automotive Grade Linux Tags API
  slug: automotive-grade-linux-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automotive-grade-linux/refs/heads/main/openapi/automotive-grade-linux-tags-api-openapi.yml
- filename: automotive-grade-linux-venues-api-openapi.yml
  format: yaml
  label: Automotive Grade Linux Venues API
  slug: automotive-grade-linux-venues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automotive-grade-linux/refs/heads/main/openapi/automotive-grade-linux-venues-api-openapi.yml
auth_types:
- http
- token
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Automotive Grade Linux Authentication
name_suffix: Authentication
oauth_flows: []
overview: Automotive Grade Linux secures its APIs with http and token across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Automotive Grade Linux
provider_slug: automotive-grade-linux
scheme_count: 2
schemes:
- anonymous_read: true
  applies_to: all write operations (POST, PUT, DELETE)
  implementation: WordPress Application Passwords. The site's /wp-json/ root advertises authentication.application-passwords.endpoints.authorization = https://www.automotivelinux.org/wp-admin/authorize-application.php
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/automotive-grade-linux-events-tec-v1-openapi.json
  - https://www.automotivelinux.org/wp-json/
  surface: AGL Events API (tec/v1 and tribe/events/v1)
  type: http
- also_used_by: the legacy XML-RPC root, as https://<user>:<token>@lava.automotivelinux.org/RPC2
  applies_to: job submission, cancellation and all writes; GET on jobs/, devices/, devicetypes/ is anonymous
  authorization_model: Token identity is separate from object permission. AGL warns that a 401/403 on LAVA can mean the token is fine but the identity lacks per-device or per-devicetype submit permission - an important distinction for an agent deciding whether to retry with a different credential or stop.
  expiry: none; static until revoked
  header: Authorization
  in: header
  name: LavaToken
  rotation: manual - created and revoked in the LAVA web UI under API > Authentication Tokens
  sources:
  - skills/automotive-grade-linux-lava-skill.md
  surface: AGL LAVA Test Lab API
  type: apiKey
  value_prefix: 'Token '
slug: automotive-grade-linux-authentication
source_filename: automotive-grade-linux-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: searched\nsource: >-\n  openapi/automotive-grade-linux-events-tec-v1-openapi.json (securitySchemes),\n  https://www.automotivelinux.org/wp-json/ (authentication block in the WordPress REST root),\n  skills/automotive-grade-linux-lava-skill.md (AGL's own auth section), and live anonymous probes\n  on 2026-09-14\ndocs:\n- https://raw.githubusercontent.com/automotive-grade-linux/lava-mcp-toolkit/main/lava-skill.md\n- https://www.automotivelinux.org/wp-json/tec/v1/docs\nsummary:\n  types:\n  - http\n  - token\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  note: >-\n    No OAuth, no OIDC, no mTLS anywhere in the AGL estate. All six hosts probed return 404 for\n    /.well-known/openid-configuration, /.well-known/oauth-authorization-server and\n    /.well-known/oauth-protected-resource, and AGL's own LAVA reference states plainly:\n    \"No OAuth, no refresh flow. Tokens are static until revoked in the UI.\"\nschemes:\n- name: BasicAuth\n\
  \  type: http\n  scheme: basic\n  surface: AGL Events API (tec/v1 and tribe/events/v1)\n  applies_to: all write operations (POST, PUT, DELETE)\n  anonymous_read: true\n  implementation: >-\n    WordPress Application Passwords. The site's /wp-json/ root advertises\n    authentication.application-passwords.endpoints.authorization =\n    https://www.automotivelinux.org/wp-admin/authorize-application.php\n  sources:\n  - openapi/automotive-grade-linux-events-tec-v1-openapi.json\n  - https://www.automotivelinux.org/wp-json/\n- name: LavaToken\n  type: apiKey\n  in: header\n  header: Authorization\n  value_prefix: \"Token \"\n  surface: AGL LAVA Test Lab API\n  applies_to: job submission, cancellation and all writes; GET on jobs/, devices/, devicetypes/ is anonymous\n  rotation: manual - created and revoked in the LAVA web UI under API > Authentication Tokens\n  expiry: none; static until revoked\n  also_used_by: the legacy XML-RPC root, as https://<user>:<token>@lava.automotivelinux.org/RPC2\n\
  \  authorization_model: >-\n    Token identity is separate from object permission. AGL warns that a 401/403 on LAVA can mean the\n    token is fine but the identity lacks per-device or per-devicetype submit permission - an important\n    distinction for an agent deciding whether to retry with a different credential or stop.\n  sources:\n  - skills/automotive-grade-linux-lava-skill.md\ncredential_handling_guidance:\n  published: true\n  detail: >-\n    Unusually for this catalog, AGL publishes guidance on where an agent's credential should live.\n    lava-skill.md opens with \"Do not embed credentials in prompts, code, or committed files\" and gives\n    a three-row table of where the token lives per access method: an environment variable for MCP\n    stdio, a server-side users.json mapping for the multi-tenant MCP server (the caller presents a\n    different bearer token that the server exchanges), and $LAVA_TOKEN / $LAVA_TOKEN_FILE /\n    ~/.config/lava/token for the shell scripts.\n\
  \  source: skills/automotive-grade-linux-lava-skill.md\nanonymous_surfaces:\n- url: https://www.automotivelinux.org/wp-json/tribe/events/v1/events\n  status: 200\n- url: https://www.automotivelinux.org/wp-json/tribe/events/v1/venues\n  status: 200\n- url: https://www.automotivelinux.org/wp-json/tec/v1/docs\n  status: 200\n- url: https://lava.automotivelinux.org/api/v0.2/\n  status: 200\n- url: https://lava.automotivelinux.org/api/v0.2/jobs/?format=json&limit=1\n  status: 200\n- url: https://gerrit.automotivelinux.org/gerrit/projects/\n  status: 200\ngated_surfaces:\n- url: https://www.automotivelinux.org/wp-json/wp-abilities/v1/abilities\n  status: 401\n  code: rest_forbidden\n- url: https://www.automotivelinux.org/wp-json/tribe/power-automate/v1/new-events\n  status: 401\n- url: https://www.automotivelinux.org/wp-json/tec/v1/events/calendar-embed\n  status: 401\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/automotive-grade-linux/refs/heads/main/authentication/automotive-grade-linux-authentication.yml
summary_line: http/token · 2 schemes
tags:
- Automotive
- Connected Vehicles
- Embedded Linux
- In-Vehicle Infotainment
- IoT
- Linux Foundation
- Open-Source
- Software Defined Vehicles
---
