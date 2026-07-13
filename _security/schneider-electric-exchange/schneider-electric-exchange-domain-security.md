---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: se.com
  spf: true
hosts:
- cert_expires: Jan 11 23:59:59 2027 GMT
  host: devportal.exchange.se.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 11 23:59:59 2027 GMT
  host: exchange.se.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 23:59:59 2026 GMT
  host: community.se.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Schneider Electric Exchange Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Schneider Electric Exchange, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Schneider Electric Exchange
provider_slug: schneider-electric-exchange
slug: schneider-electric-exchange-domain-security
source_filename: schneider-electric-exchange-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: devportal.exchange.se.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: exchange.se.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: community.se.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: se.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/schneider-electric-exchange/refs/heads/main/security/schneider-electric-exchange-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Building Automation
- Commerce APIs
- EcoStruxure
- Energy Management
- Industrial IoT
- Schneider Electric
---
