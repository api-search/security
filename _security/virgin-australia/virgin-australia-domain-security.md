---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: virginaustralia.com
  spf: true
hosts:
- cert_expires: Mar 24 23:59:59 2027 GMT
  host: www.virginaustralia.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Virgin Australia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Virgin Australia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Virgin Australia
provider_slug: virgin-australia
slug: virgin-australia-domain-security
source_filename: virgin-australia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.virginaustralia.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 24 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: virginaustralia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/virgin-australia/refs/heads/main/security/virgin-australia-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Travel
- Australia
- Aviation
- Airlines
- Distribution
- GDS
- NDC
- Booking
- Loyalty
- Corporate Travel
---
