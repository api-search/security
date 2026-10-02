---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: richapi.ai
  spf: false
hosts:
- cert_expires: Nov 10 14:07:12 2026 GMT
  host: richapi.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Richapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RichAPI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: RichAPI
provider_slug: richapi
slug: richapi-domain-security
source_filename: richapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: richapi.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 14:07:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: richapi.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/richapi/refs/heads/main/security/richapi-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- API
- Data-Enrichment
- B2B
- MCP
---
