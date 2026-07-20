---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: airspacelink.com
  spf: true
hosts:
- cert_expires: Sep  2 22:58:12 2026 GMT
  host: airspacelink.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 00:02:30 2026 GMT
  host: developers.airspacelink.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: airhub-api.airspacelink.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Airspace Link Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Airspace Link, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Airspace Link
provider_slug: airspace-link
slug: airspace-link-domain-security
source_filename: airspace-link-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: airspacelink.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 22:58:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.airspacelink.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  1 00:02:30 2026 GMT\n  hsts: false\n- host: airhub-api.airspacelink.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: airspacelink.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airspace-link/refs/heads/main/security/airspace-link-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Drones
- UAS
- Airspace
- Aviation
- LAANC
- UTM
- Geospatial
- Public Safety
- Logistics
---
