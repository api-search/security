---
api_specs:
- filename: instant-answer-openapi.yml
  format: yaml
  label: DuckDuckGo Instant Answer API
  slug: instant-answer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duckduckgo/refs/heads/main/openapi/instant-answer-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: duckduckgo.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: duck.ai
  spf: false
hosts:
- cert_expires: Nov 19 23:59:59 2026 GMT
  host: duckduckgo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 19 23:59:59 2026 GMT
  host: api.duckduckgo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 02:23:36 2026 GMT
  host: duck.ai
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Duckduckgo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DuckDuckGo, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: DuckDuckGo
provider_slug: duckduckgo
slug: duckduckgo-domain-security
source_filename: duckduckgo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: duckduckgo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.duckduckgo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: duck.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 02:23:36 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: duckduckgo.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: duck.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/duckduckgo/refs/heads/main/security/duckduckgo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Search
- Privacy
- Browser
- AI Chat
- Email Protection
- VPN
- Trackers
- Identity
---
