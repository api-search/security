---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: augmodo.com
  spf: true
hosts:
- cert_expires: Nov 19 05:07:02 2026 GMT
  host: www.augmodo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Augmodo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Augmodo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Augmodo
provider_slug: augmodo
slug: augmodo-domain-security
source_filename: augmodo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.augmodo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 05:07:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: augmodo.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/augmodo/refs/heads/main/security/augmodo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Retail
- Spatial AI
- Smartbadge
- Supply chain
- Compliance
---
