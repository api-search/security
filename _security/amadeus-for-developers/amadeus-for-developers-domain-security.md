---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: amadeus.com
  spf: true
hosts:
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: developers.amadeus.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Amadeus For Developers Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amadeus for Developers, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Amadeus for Developers
provider_slug: amadeus-for-developers
slug: amadeus-for-developers-domain-security
source_filename: amadeus-for-developers-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.amadeus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: amadeus.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amadeus-for-developers/refs/heads/main/security/amadeus-for-developers-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Transportation
- Public APIs
---
