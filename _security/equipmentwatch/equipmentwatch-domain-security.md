---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: equipmentwatch.com
  spf: true
hosts:
- cert_expires: Sep 14 13:29:40 2026 GMT
  host: www.equipmentwatch.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Equipmentwatch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Equipmentwatch, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Equipmentwatch
provider_slug: equipmentwatch
slug: equipmentwatch-domain-security
source_filename: equipmentwatch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.equipmentwatch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 13:29:40 2026 GMT\n  hsts: false\ndomains:\n- domain: equipmentwatch.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/equipmentwatch/refs/heads/main/security/equipmentwatch-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Construction
- Equipment
- Rental Rates
- Valuation
- Heavy Equipment
---
