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
  dmarc_policy: reject
  dnssec: false
  domain: spotio.com
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: spotio2.com
  spf: false
hosts:
- cert_expires: Sep 30 18:44:24 2026 GMT
  host: spotio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 14:25:17 2026 GMT
  host: developer.spotio2.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 17:33:24 2026 GMT
  host: support.spotio.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spotio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SPOTIO, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SPOTIO
provider_slug: spotio
slug: spotio-domain-security
source_filename: spotio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spotio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 18:44:24 2026 GMT\n  hsts: false\n- host: developer.spotio2.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 14:25:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: support.spotio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 17:33:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: spotio.com\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: spotio2.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spotio/refs/heads/main/security/spotio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Field Sales
- Sales Engagement
- Territory Management
- CRM
- Lead Tracking
- Outside Sales
- Sales Enablement
---
