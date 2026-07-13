---
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: aveva.com
  spf: true
hosts:
- cert_expires: Aug 13 02:48:12 2026 GMT
  host: www.aveva.com
  hsts: true
  hsts_max_age: 15638400
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 06:41:07 2026 GMT
  host: docs.aveva.com
  hsts: true
  hsts_max_age: 15638400
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 24 23:59:59 2027 GMT
  host: api.connect.aveva.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aveva Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AVEVA, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AVEVA
provider_slug: aveva
slug: aveva-domain-security
source_filename: aveva-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aveva.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 02:48:12 2026 GMT\n  hsts: true\n  hsts_max_age: 15638400\n- host: docs.aveva.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 06:41:07 2026 GMT\n  hsts: true\n  hsts_max_age: 15638400\n- host: api.connect.aveva.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 24 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: aveva.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aveva/refs/heads/main/security/aveva-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- SCADA
- MES
- Industrial Automation
- Manufacturing
- Industrial IoT
- IIoT
- Industrial Data
- Energy
---
