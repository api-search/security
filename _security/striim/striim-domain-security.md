---
description: ''
domains:
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
- cert_expires: Oct  6 22:17:08 2026 GMT
  host: striim.stoplight.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Striim Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Striim, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Striim
provider_slug: striim
slug: striim-domain-security
source_filename: striim-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: striim.stoplight.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 22:17:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: stoplight.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:devops@stoplight.io\"\n  - 0 issue \"cloudflare.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/striim/refs/heads/main/security/striim-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data
- Streaming
- Change Data Capture
- Real-time
- Data Integration
- Streaming Analytics
---
