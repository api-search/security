---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: schiphol.nl
  spf: true
hosts:
- cert_expires: Aug 26 07:59:14 2026 GMT
  host: developer.schiphol.nl
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Schiphol Airport Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Schiphol Airport, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Schiphol Airport
provider_slug: schiphol-airport
slug: schiphol-airport-domain-security
source_filename: schiphol-airport-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.schiphol.nl\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 26 07:59:14 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: schiphol.nl\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/schiphol-airport/refs/heads/main/security/schiphol-airport-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Transportation
- Public APIs
---
