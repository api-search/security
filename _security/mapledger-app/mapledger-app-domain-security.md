---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mapledger.app
  spf: true
hosts:
- cert_expires: Dec 20 16:51:46 2026 GMT
  host: mapledger.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MapLedger Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MapLedger, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: MapLedger
provider_slug: mapledger-app
slug: mapledger-app-domain-security
source_filename: mapledger-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mapledger.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 16:51:46 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mapledger.app\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/mapledger-app/security/mapledger-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data
- Real Estate
- Zoning
- Business Directory
---
