---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: andes.bio
  spf: true
hosts:
- cert_expires: Oct 13 19:26:46 2026 GMT
  host: www.andes.bio
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Andes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Andes, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Andes
provider_slug: andes
slug: andes-domain-security
source_filename: andes-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.andes.bio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 19:26:46 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: andes.bio\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/andes/refs/heads/main/security/andes-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Climate
- Carbon Removal
- Agriculture
- Agriculture Technology
- Biotechnology
- Sustainability
- Carbon Credits
- Soil
---
