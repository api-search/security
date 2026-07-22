---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: smart-bricks.com
  spf: true
hosts:
- cert_expires: Mar  7 23:59:59 2027 GMT
  host: smart-bricks.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Smart Bricks Holdings Limited Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Smart Bricks Holdings Limited, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Smart Bricks Holdings Limited
provider_slug: smart-bricks-holdings-limited
slug: smart-bricks-holdings-limited-domain-security
source_filename: smart-bricks-holdings-limited-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: smart-bricks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: smart-bricks.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smart-bricks-holdings-limited/refs/heads/main/security/smart-bricks-holdings-limited-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Real Estate
- PropTech
- Artificial Intelligence
- Investment
- Autonomous Agents
- FinTech
---
