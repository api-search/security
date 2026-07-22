---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: preql.ai
  spf: false
hosts:
- cert_expires: Oct 14 15:51:43 2026 GMT
  host: www.preql.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Preql Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Preql, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Preql
provider_slug: preql
slug: preql-domain-security
source_filename: preql-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.preql.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 15:51:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: preql.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/preql/refs/heads/main/security/preql-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Developer
- Data
- Artificial Intelligence
- Analytics
- Data Cleaning
- Semantic Modeling
- Enterprise
---
