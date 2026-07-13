---
api_specs:
- filename: gong-calls-openapi.yml
  format: yaml
  label: Gong Calls API
  slug: gong-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gong/refs/heads/main/openapi/gong-calls-openapi.yml
- filename: gong-users-openapi.yml
  format: yaml
  label: Gong Users API
  slug: gong-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gong/refs/heads/main/openapi/gong-users-openapi.yml
- filename: gong-library-openapi.yml
  format: yaml
  label: Gong Library API
  slug: gong-library-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gong/refs/heads/main/openapi/gong-library-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gong.io
  spf: true
hosts:
- cert_expires: Sep 11 14:04:16 2026 GMT
  host: www.gong.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 01:44:06 2026 GMT
  host: app.gong.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 15:19:55 2026 GMT
  host: api.gong.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gong Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gong, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Gong
provider_slug: gong
slug: gong-domain-security
source_filename: gong-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gong.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 14:04:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.gong.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 01:44:06 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.gong.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 15:19:55 2026 GMT\n  hsts: null\ndomains:\n- domain: gong.io\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gong/refs/heads/main/security/gong-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Sales
- Revenue Intelligence
- Conversation
- Analytics
- AI
---
