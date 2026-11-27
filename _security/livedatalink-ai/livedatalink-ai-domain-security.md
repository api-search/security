---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: livedatalink.ai
  spf: true
hosts:
- cert_expires: Feb 12 16:07:21 2027 GMT
  host: livedatalink.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: LiveDataLink Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LiveDataLink, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: LiveDataLink
provider_slug: livedatalink-ai
slug: livedatalink-ai-domain-security
source_filename: livedatalink-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: livedatalink.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 12 16:07:21 2027 GMT\n  hsts: false\ndomains:\n- domain: livedatalink.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/livedatalink-ai/security/livedatalink-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Data
- Artificial Intelligence
- Public Data
- MCP
- Aggregation
---
