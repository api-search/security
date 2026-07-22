---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: graphenest.com
  spf: true
hosts:
- cert_expires: Mar  5 23:59:59 2027 GMT
  host: graphenest.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Graphenestcom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for graphenest.com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: graphenest.com
provider_slug: graphenestcom
slug: graphenestcom-domain-security
source_filename: graphenestcom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: graphenest.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  5 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: graphenest.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/graphenestcom/refs/heads/main/security/graphenestcom-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Graphene
- Nanotechnology
- Advanced Materials
- EMI Shielding
- Electromagnetic Compatibility
- Conductive Coatings
- Cleantech
- Manufacturing
---
