---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cyclicmaterials.earth
  spf: true
hosts:
- cert_expires: Nov  8 02:24:22 2026 GMT
  host: cyclicmaterials.earth
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cyclic Materials Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cyclic Materials, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cyclic Materials
provider_slug: cyclic-materials
slug: cyclic-materials-domain-security
source_filename: cyclic-materials-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cyclicmaterials.earth\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 02:24:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cyclicmaterials.earth\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cyclic-materials/refs/heads/main/security/cyclic-materials-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Rare Earth Elements
- Critical Minerals
- Recycling
- Circular Economy
- Cleantech
- Advanced Materials
- Sustainability
---
