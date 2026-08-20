---
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: zemanta.com
  spf: true
hosts:
- cert_expires: Nov 28 23:59:59 2026 GMT
  host: zemanta.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 08:04:12 2026 GMT
  host: dev.zemanta.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 22:23:35 2026 GMT
  host: oneapi.zemanta.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zemanta Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zemanta, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Zemanta
provider_slug: zemanta
slug: zemanta-domain-security
source_filename: zemanta-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zemanta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dev.zemanta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 08:04:12 2026 GMT\n  hsts: false\n- host: oneapi.zemanta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 22:23:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: zemanta.com\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zemanta/refs/heads/main/security/zemanta-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Advertising
- Native Advertising
- Programmatic
- DSP
- AdTech
- Content Recommendation
- Marketing
- Campaign Management
- Demand-Side Platform
- Media Buying
---
