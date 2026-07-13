---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ubixlabs.com
  spf: true
hosts:
- cert_expires: Sep  3 07:01:20 2026 GMT
  host: www.ubixlabs.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.ubixlabs.com
  https: false
kind: domain-security
layout: security
method: probed
name: Ubix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UBIX Labs, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: UBIX Labs
provider_slug: ubix
slug: ubix-domain-security
source_filename: ubix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ubixlabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 07:01:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.ubixlabs.com\n  https: false\ndomains:\n- domain: ubixlabs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ubix/refs/heads/main/security/ubix-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Analytics
- Machine Learning
- Data Integration
- No-Code
- Enterprise
- Generative AI
---
