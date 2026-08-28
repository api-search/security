---
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: life360.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nativo.com
  spf: true
hosts:
- cert_expires: Nov 16 11:12:04 2026 GMT
  host: ads.life360.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 20 04:58:59 2026 GMT
  host: api-docs.nativo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 17:06:09 2026 GMT
  host: api.nativo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nativo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nativo, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Nativo
provider_slug: nativo
slug: nativo-domain-security
source_filename: nativo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ads.life360.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 11:12:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-docs.nativo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 04:58:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.nativo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 17:06:09 2026 GMT\n  hsts: null\ndomains:\n- domain: life360.com\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: nativo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nativo/refs/heads/main/security/nativo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Advertising
- AdTech
- Native Advertising
- Programmatic Advertising
- Supply Side Platform
- Ad Serving
- Marketing
- Publishing
- Reporting
- Mobile SDK
---
