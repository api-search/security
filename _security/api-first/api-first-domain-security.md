---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: swagger.io
  spf: true
- caa:
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:devops@stoplight.io"
  - 0 issue "cloudflare.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: stoplight.io
  spf: true
hosts:
- cert_expires: Oct  4 16:46:01 2026 GMT
  host: swagger.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 22:17:08 2026 GMT
  host: stoplight.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 09:00:12 2026 GMT
  host: www.postman.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Api First Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for API-First, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: API-First
provider_slug: api-first
slug: api-first-domain-security
source_filename: api-first-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: swagger.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 16:46:01 2026 GMT\n  hsts: false\n- host: stoplight.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 22:17:08 2026 GMT\n  hsts: false\n- host: www.postman.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 09:00:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: swagger.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: stoplight.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:devops@stoplight.io\"\n  - 0 issue \"cloudflare.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/api-first/refs/heads/main/security/api-first-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API Design
- Development Methodology
- Software Architecture
- API Governance
- Microservices
---
