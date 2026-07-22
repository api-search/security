---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: noviconnect.com
  spf: true
hosts:
- cert_expires: Oct  1 09:48:29 2026 GMT
  host: www.noviconnect.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Novi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Novi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Novi
provider_slug: novi
slug: novi-domain-security
source_filename: novi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.noviconnect.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 09:48:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: noviconnect.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/novi/refs/heads/main/security/novi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Commerce
- Retail
- Consumer Packaged Goods
- Product Data
- E-Commerce
- Agentic Search
---
