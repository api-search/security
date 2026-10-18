---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cuddly.com
  spf: true
hosts:
- cert_expires: Apr  8 23:59:59 2027 GMT
  host: cuddly.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cuddly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CUDDLY, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CUDDLY
provider_slug: cuddly
slug: cuddly-domain-security
source_filename: cuddly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cuddly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  8 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cuddly.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cuddly/refs/heads/main/security/cuddly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Crowdfunding
- Animal Welfare
- Non-Profit
- E-Commerce
---
