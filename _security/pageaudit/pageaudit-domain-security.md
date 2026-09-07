---
api_specs:
- filename: openapi.json
  format: json
  label: PageAudit API
  slug: pageaudit-api
  spec_type: OpenAPI
  url: https://pageaudit.online/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pageaudit.online
  spf: true
hosts:
- cert_expires: Nov  8 23:55:20 2026 GMT
  host: pageaudit.online
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Pageaudit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PageAudit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: PageAudit
provider_slug: pageaudit
slug: pageaudit-domain-security
source_filename: pageaudit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pageaudit.online\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 23:55:20 2026 GMT\n  hsts: false\ndomains:\n- domain: pageaudit.online\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pageaudit/refs/heads/main/security/pageaudit-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Technical SEO
- SEO auditing
- Developer Tools
- Agent-native
- MCP
- x402
---
