---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mobis.com
  spf: true
hosts:
- cert_expires: Mar  8 23:59:59 2027 GMT
  host: www.mobis.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Hyundai Mobis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hyundai Mobis, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Hyundai Mobis
provider_slug: hyundai-mobis
slug: hyundai-mobis-domain-security
source_filename: hyundai-mobis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mobis.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  8 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: mobis.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hyundai-mobis/refs/heads/main/security/hyundai-mobis-domain-security.yml
summary_line: TLSv1.2
tags:
- Automotive
- Tier 1 Supplier
- Modules
- ADAS
- Electrification
- Hyundai Group
---
