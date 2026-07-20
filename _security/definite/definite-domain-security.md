---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: definite.app
  spf: true
hosts:
- cert_expires: Sep 29 18:40:13 2026 GMT
  host: www.definite.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 16:13:05 2026 GMT
  host: api.definite.app
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Definite Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Definite, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Definite
provider_slug: definite
slug: definite-domain-security
source_filename: definite-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.definite.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 18:40:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.definite.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 16:13:05 2026 GMT\n  hsts: null\ndomains:\n- domain: definite.app\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/definite/refs/heads/main/security/definite-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Data
- Analytics
- Business Intelligence
- Data Integration
- Data Warehouse
- Lakehouse
- Semantic Layer
- Artificial Intelligence
- AI Agents
- Model Context Protocol
- ETL
---
