---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: false
  dnssec: false
  domain: mostly.ai
  spf: true
hosts:
- cert_expires: Sep 30 12:28:35 2026 GMT
  host: mostly.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api-docs.mostly.ai
  https: false
- host: app.mostly.ai
  https: false
kind: domain-security
layout: security
method: probed
name: Mostly Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MOSTLY AI, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: MOSTLY AI
provider_slug: mostly-ai
slug: mostly-ai-domain-security
source_filename: mostly-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mostly.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 12:28:35 2026 GMT\n  hsts: false\n- host: api-docs.mostly.ai\n  https: false\n- host: app.mostly.ai\n  https: false\ndomains:\n- domain: mostly.ai\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mostly-ai/refs/heads/main/security/mostly-ai-domain-security.yml
summary_line: TLSv1.3
tags:
- Synthetic Data
- Privacy
- Tabular
- Differential Privacy
- Python SDK
- REST
- Apache 2.0
---
