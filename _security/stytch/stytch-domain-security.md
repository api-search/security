---
api_specs:
- filename: stytch-consumer-openapi.yml
  format: yaml
  label: Stytch Consumer Authentication API
  slug: stytch-consumer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stytch/refs/heads/main/openapi/stytch-consumer-openapi.yml
- filename: stytch-b2b-openapi.yml
  format: yaml
  label: Stytch B2B Authentication API
  slug: stytch-b2b-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stytch/refs/heads/main/openapi/stytch-b2b-openapi.yml
- filename: stytch-management-openapi.yml
  format: yaml
  label: Stytch Management API
  slug: stytch-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stytch/refs/heads/main/openapi/stytch-management-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: stytch.com
  spf: true
hosts:
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: stytch.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: app.stytch.com
  https: false
- cert_expires: Oct  7 23:59:59 2026 GMT
  host: api.stytch.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stytch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stytch, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Stytch
provider_slug: stytch
slug: stytch-domain-security
source_filename: stytch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: stytch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.stytch.com\n  https: false\n- host: api.stytch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: stytch.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stytch/refs/heads/main/security/stytch-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Authentication
- Identity
- Passwordless
- Security
- B2B
- Connected Apps
- MCP
- AI Agents
- Developer Tools
---
