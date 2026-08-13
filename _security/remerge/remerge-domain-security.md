---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: remerge.events
  spf: true
  spf_record: v=spf1 -all
- caa:
  - 0 issue "digicert.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: remerge.io
  spf: true
hosts:
- cert_expires: Oct  5 12:17:47 2026 GMT
  host: www.remerge.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 23:43:49 2026 GMT
  host: help.remerge.io
  hsts: true
  hsts_max_age: 259200
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 20 23:59:59 2027 GMT
  host: api.remerge.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 20 23:59:59 2027 GMT
  cert_issuer: DigiCert Global G2 TLS RSA SHA256 2020 CA1
  host: remerge.events
  hsts: false
  https: true
  note: Event Tracking API host. Added by hand on 2026-08-12 — probe-domain-security.py walks apis.yml/OpenAPI hosts under the primary domain and skipped this second registrable domain. Values are live probes of remerge.events.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Remerge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Remerge, probed live across 4 host(s) and 2 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Remerge
provider_slug: remerge
slug: remerge-domain-security
source_filename: remerge-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.remerge.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 12:17:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.remerge.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 23:43:49 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\n- host: api.remerge.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 20 23:59:59 2027 GMT\n  hsts: null\n- host: remerge.events\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 20 23:59:59 2027 GMT\n  cert_issuer: DigiCert Global G2 TLS RSA SHA256 2020 CA1\n  hsts: false\n  note: >-\n    Event Tracking API host. Added by hand on 2026-08-12 — probe-domain-security.py\n    walks apis.yml/OpenAPI hosts under the primary domain and skipped this\n    second registrable domain. Values are live probes of remerge.events.\ndomains:\n- domain: remerge.events\n  dnssec:\
  \ false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  spf_record: v=spf1 -all\n  dmarc: true\n  dmarc_policy: reject\n- domain: remerge.io\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/remerge/refs/heads/main/security/remerge-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Advertising
- AdTech
- Mobile
- Retargeting
- Demand-Side Platform
- User Acquisition
- Marketing
---
