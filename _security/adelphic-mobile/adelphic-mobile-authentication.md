---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: probed
name: Adelphic Mobile Authentication
name_suffix: Authentication
oauth_flows: []
overview: Adelphic Mobile * secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Adelphic Mobile *
provider_slug: adelphic-mobile
scheme_count: 1
schemes:
- description: 'HTTP Basic authentication. Probing https://api.adelphic.com/ returns 401 Unauthorized with header `WWW-Authenticate: Basic realm="Adelphic"`. Credentials are provisioned to enterprise Adelphic DSP accounts.'
  name: basicAuth
  observed:
    host: https://api.adelphic.com
    server: Apache Tomcat
    status: 401
    www_authenticate: Basic realm="Adelphic"
  scheme: basic
  sources:
  - live probe of https://api.adelphic.com/ on 2026-07-17
  type: http
slug: adelphic-mobile-authentication
source_filename: adelphic-mobile-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live HTTP probe of https://api.adelphic.com/ (WWW-Authenticate response header)\nsummary:\n  types:\n  - http\n  note: >-\n    Adelphic publishes no public OpenAPI or self-service developer auth\n    reference. This profile records what was directly observed by probing the\n    live API host api.adelphic.com, a gated enterprise endpoint (Apache Tomcat)\n    protected by HTTP Basic authentication. Access requires Viant/Adelphic\n    account credentials; there is no public key issuance.\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: >-\n    HTTP Basic authentication. Probing https://api.adelphic.com/ returns\n    401 Unauthorized with header `WWW-Authenticate: Basic realm=\"Adelphic\"`.\n    Credentials are provisioned to enterprise Adelphic DSP accounts.\n  observed:\n    host: https://api.adelphic.com\n    status: 401\n    www_authenticate: Basic realm=\"Adelphic\"\n    server: Apache Tomcat\n  sources:\n\
  \  - live probe of https://api.adelphic.com/ on 2026-07-17\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adelphic-mobile/refs/heads/main/authentication/adelphic-mobile-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Enterprise
- Advertising
- AdTech
- Programmatic Advertising
- Demand Side Platform
- DSP
- Marketing
- Connected TV
---
