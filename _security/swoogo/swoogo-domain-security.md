---
api_specs:
- filename: swoogo-openapi.yml
  format: yaml
  label: Swoogo Events API
  slug: swoogo-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swoogo/refs/heads/main/openapi/swoogo-openapi.yml
- filename: swoogo-openapi.yml
  format: yaml
  label: Swoogo Registrants API
  slug: swoogo-registrants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swoogo/refs/heads/main/openapi/swoogo-openapi.yml
- filename: swoogo-openapi.yml
  format: yaml
  label: Swoogo Sessions API
  slug: swoogo-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swoogo/refs/heads/main/openapi/swoogo-openapi.yml
- filename: swoogo-openapi.yml
  format: yaml
  label: Swoogo Speakers API
  slug: swoogo-speakers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swoogo/refs/heads/main/openapi/swoogo-openapi.yml
- filename: swoogo-openapi.yml
  format: yaml
  label: Swoogo Contacts API
  slug: swoogo-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swoogo/refs/heads/main/openapi/swoogo-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: swoogo.events
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: readme.io
  spf: true
hosts:
- cert_expires: Sep 14 05:33:04 2026 GMT
  host: swoogo.events
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 13:12:37 2026 GMT
  host: swoogo.readme.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 12 23:59:59 2027 GMT
  host: api.swoogo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Swoogo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Swoogo, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Swoogo
provider_slug: swoogo
slug: swoogo-domain-security
source_filename: swoogo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: swoogo.events\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 05:33:04 2026 GMT\n  hsts: false\n- host: swoogo.readme.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 13:12:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.swoogo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 12 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: swoogo.events\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n- domain: readme.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swoogo/refs/heads/main/security/swoogo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Event Management
- Event Registration
- Events
- Sessions
- Speakers
- Attendees
- SaaS
---
