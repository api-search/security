---
description: ''
domains:
- caa:
  - 0 issue "anf.es"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: flanks.io
  spf: true
hosts:
- cert_expires: Sep  3 19:20:27 2026 GMT
  host: docs.flanks.io
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 19:20:27 2026 GMT
  host: api.flanks.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Flanks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flanks, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Flanks
provider_slug: flanks
slug: flanks-domain-security
source_filename: flanks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.flanks.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 19:20:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: api.flanks.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 19:20:27 2026 GMT\n  hsts: null\ndomains:\n- domain: flanks.io\n  dnssec: false\n  caa:\n  - 0 issue \"anf.es\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flanks/refs/heads/main/security/flanks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Wealth Management
- Financial Data
- Data Aggregation
- Fintech
- Investments
- Open Banking
- APIs
---
