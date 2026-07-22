---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: higharc.com
  spf: true
hosts:
- cert_expires: Oct  3 14:28:16 2026 GMT
  host: www.higharc.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Higharc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Higharc, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Higharc
provider_slug: higharc
slug: higharc-domain-security
source_filename: higharc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.higharc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 14:28:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: higharc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/higharc/refs/heads/main/security/higharc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Construction Tech
- Homebuilding
- Artificial Intelligence
- Construction
- Design
- 3D Visualization
- Estimating
- PropTech
- SaaS
---
