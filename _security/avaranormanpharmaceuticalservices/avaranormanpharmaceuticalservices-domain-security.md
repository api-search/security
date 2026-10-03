---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: avara.com
  spf: true
hosts:
- cert_expires: Nov  9 12:41:27 2026 GMT
  host: www.avara.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Avaranormanpharmaceuticalservices Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Avaranormanpharmaceuticalservices, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Avaranormanpharmaceuticalservices
provider_slug: avaranormanpharmaceuticalservices
slug: avaranormanpharmaceuticalservices-domain-security
source_filename: avaranormanpharmaceuticalservices-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.avara.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 12:41:27 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: avara.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avaranormanpharmaceuticalservices/refs/heads/main/security/avaranormanpharmaceuticalservices-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Pharmaceuticals
- Services
- Healthcare
- Biotechnology
---
