---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: olx.pl
  spf: true
hosts:
- cert_expires: Oct 14 23:59:59 2026 GMT
  host: developer.olx.pl
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Olx Poland Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OLX Poland, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: OLX Poland
provider_slug: olx-poland
slug: olx-poland-domain-security
source_filename: olx-poland-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.olx.pl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: olx.pl\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/olx-poland/refs/heads/main/security/olx-poland-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Shopping
- Public APIs
---
