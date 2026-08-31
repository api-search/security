---
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "certainly.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: voi.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: voiapp.io
  spf: true
hosts:
- cert_expires: Sep 21 08:17:22 2026 GMT
  host: www.voi.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 12:21:39 2026 GMT
  host: partners.voiapp.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 12:21:39 2026 GMT
  host: mds.voiapp.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Voi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Voi, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Voi
provider_slug: voi
slug: voi-domain-security
source_filename: voi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.voi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 08:17:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: partners.voiapp.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 12:21:39 2026 GMT\n  hsts: null\n- host: mds.voiapp.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 12:21:39 2026 GMT\n  hsts: null\ndomains:\n- domain: voi.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"certainly.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: voiapp.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voi/refs/heads/main/security/voi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Micromobility
- E-Scooters
- E-Bikes
- Mobility-as-a-Service
- Transportation
- GBFS
- MDS
- Sweden
---
