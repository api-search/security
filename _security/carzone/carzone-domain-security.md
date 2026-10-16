---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: carzone.ie
  spf: true
hosts:
- cert_expires: Nov 14 19:03:40 2026 GMT
  host: www.carzone.ie
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Carzone Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Carzone, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Carzone
provider_slug: carzone
slug: carzone-domain-security
source_filename: carzone-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.carzone.ie\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 19:03:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: carzone.ie\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carzone/refs/heads/main/security/carzone-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Marketplace
- Automotive
- Ireland
- Cars
---
