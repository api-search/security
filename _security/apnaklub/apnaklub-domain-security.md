---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: apnaklub.com
  spf: true
hosts:
- cert_expires: Nov 28 05:40:23 2026 GMT
  host: www.apnaklub.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Apnaklub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apnaklub, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Apnaklub
provider_slug: apnaklub
slug: apnaklub-domain-security
source_filename: apnaklub-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.apnaklub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 05:40:23 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: apnaklub.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apnaklub/refs/heads/main/security/apnaklub-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- B2B
- Retail
- FMCG
- India
- Marketplace
---
