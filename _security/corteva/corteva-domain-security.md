---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: corteva.com
  spf: true
hosts:
- cert_expires: Sep  2 12:33:44 2026 GMT
  host: www.corteva.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Corteva Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Corteva, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Corteva
provider_slug: corteva
slug: corteva-domain-security
source_filename: corteva-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.corteva.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 12:33:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: corteva.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/corteva/refs/heads/main/security/corteva-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Agriculture
- Agriscience
- Biologicals
- Crop Protection
- DowDuPont
- Farm Management
- Farming
- Fortune 500
- Fungicides
- Granular
- Herbicides
- Insecticides
- Pioneer
- Seeds
---
