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
  dmarc_policy: quarantine
  dnssec: false
  domain: voi.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: voiscooters.com
  spf: true
hosts:
- cert_expires: Sep 21 08:17:22 2026 GMT
  host: www.voi.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: docs.voiscooters.com
  https: false
kind: domain-security
layout: security
method: probed
name: Voi App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Voi, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Voi
provider_slug: voi-app
slug: voi-app-domain-security
source_filename: voi-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.voi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 08:17:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.voiscooters.com\n  https: false\ndomains:\n- domain: voi.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: voiscooters.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voi-app/refs/heads/main/security/voi-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Micromobility
- Shared Mobility
- E-Scooters
- E-Bikes
- Transportation
- MaaS
- Mobility As A Service
- GBFS
- MDS
- Open Mobility
- Smart Cities
- Sweden
- Europe
---
