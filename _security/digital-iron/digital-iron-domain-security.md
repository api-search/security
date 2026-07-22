---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: digitaliron.com
  spf: true
hosts:
- cert_expires: Aug  3 11:38:44 2026 GMT
  host: digitaliron.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Digital Iron Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Digital Iron, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Digital Iron
provider_slug: digital-iron
slug: digital-iron-domain-security
source_filename: digital-iron-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: digitaliron.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  3 11:38:44 2026 GMT\n  hsts: false\ndomains:\n- domain: digitaliron.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/digital-iron/refs/heads/main/security/digital-iron-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Heavy Machinery
- Aftersales
- Field Service
- Equipment Dealers
- OEM
- Service Data
---
