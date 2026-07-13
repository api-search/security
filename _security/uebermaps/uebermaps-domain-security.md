---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: uebermaps.com
  spf: true
hosts:
- cert_expires: Aug 25 12:09:29 2026 GMT
  host: uebermaps.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Uebermaps Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Uebermaps, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Uebermaps
provider_slug: uebermaps
slug: uebermaps-domain-security
source_filename: uebermaps-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: uebermaps.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 12:09:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: uebermaps.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uebermaps/refs/heads/main/security/uebermaps-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Geocoding
- Public APIs
---
