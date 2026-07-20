---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: jedify.com
  spf: true
hosts:
- cert_expires: Sep 23 23:34:04 2026 GMT
  host: jedify.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 01:07:34 2026 GMT
  host: docs.jedify.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 10:49:25 2026 GMT
  host: be.jedify.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jedify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jedify, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Jedify
provider_slug: jedify
slug: jedify-domain-security
source_filename: jedify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jedify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 23:34:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.jedify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 01:07:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: be.jedify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 10:49:25 2026 GMT\n  hsts: null\ndomains:\n- domain: jedify.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jedify/refs/heads/main/security/jedify-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Data Analytics
- Business Intelligence
- Semantic Layer
- Context Layer
- Data Agents
- MCP
- Enterprise AI
- Natural Language Query
---
