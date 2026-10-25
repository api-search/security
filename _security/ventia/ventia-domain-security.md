---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ventia.com
  spf: true
hosts:
- cert_expires: Nov 14 23:11:40 2026 GMT
  host: ventia.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ventia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ventia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ventia
provider_slug: ventia
slug: ventia-domain-security
source_filename: ventia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ventia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 23:11:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: ventia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ventia/refs/heads/main/security/ventia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Infrastructure Services
- Facilities Management
- Utilities
- Transport
- Defence
- Telecommunications
- Australia
- New Zealand
---
