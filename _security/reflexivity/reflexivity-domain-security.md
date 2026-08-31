---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: reflexivity.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: tgl.ai
  spf: false
hosts:
- cert_expires: Oct 11 13:58:08 2026 GMT
  host: reflexivity.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 26 08:56:56 2026 GMT
  host: api-docs.tgl.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 13:58:08 2026 GMT
  host: api.reflexivity.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Reflexivity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Reflexivity, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Reflexivity
provider_slug: reflexivity
slug: reflexivity-domain-security
source_filename: reflexivity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: reflexivity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 13:58:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-docs.tgl.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 08:56:56 2026 GMT\n  hsts: null\n- host: api.reflexivity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 13:58:08 2026 GMT\n  hsts: null\ndomains:\n- domain: reflexivity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: tgl.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reflexivity/refs/heads/main/security/reflexivity-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Financial-Services
- Investment Analysis
- Market Data
- Artificial Intelligence
- Machine-Learning
- Fintech
- Research
- Knowledge Graph
- Agents
---
