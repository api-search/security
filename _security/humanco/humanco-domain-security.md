---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: humanco.com
  spf: true
hosts:
- cert_expires: Sep 13 16:02:45 2026 GMT
  host: www.humanco.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Humanco Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HumanCo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: HumanCo
provider_slug: humanco
slug: humanco-domain-security
source_filename: humanco-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.humanco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 16:02:45 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: humanco.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/humanco/refs/heads/main/security/humanco-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer Packaged Goods
- Food and Beverage
- Wellness
- Health
- E-Commerce
- Sustainability
- Portfolio Company
---
