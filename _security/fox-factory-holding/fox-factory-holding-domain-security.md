---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ridefox.com
  spf: true
hosts:
- cert_expires: Oct 30 15:35:01 2026 GMT
  host: ridefox.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fox Factory Holding Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fox Factory Holding, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Fox Factory Holding
provider_slug: fox-factory-holding
slug: fox-factory-holding-domain-security
source_filename: fox-factory-holding-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ridefox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 15:35:01 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: ridefox.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fox-factory-holding/refs/heads/main/security/fox-factory-holding-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Suspension
- Cycling
- Power-Sports
- Manufacturing
- E-Commerce
- MCP
- Agentic Commerce
---
