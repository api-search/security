---
api_specs:
- filename: causa-prima-scribo-openapi.json
  format: json
  label: Scribo Invoice API
  slug: causa-prima-scribo
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/causa-prima/refs/heads/main/openapi/causa-prima-scribo-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: causaprima.ai
  spf: true
hosts:
- cert_expires: Sep 10 09:54:09 2026 GMT
  host: causaprima.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 18:57:48 2026 GMT
  host: scribo.causaprima.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Causa Prima Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Causa Prima, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Causa Prima
provider_slug: causa-prima
slug: causa-prima-domain-security
source_filename: causa-prima-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: causaprima.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 09:54:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: scribo.causaprima.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 18:57:48 2026 GMT\n  hsts: false\ndomains:\n- domain: causaprima.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/causa-prima/refs/heads/main/security/causa-prima-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Fintech
- E-Invoicing
- Invoicing
- Payments
- Compliance
- Germany
- EN 16931
- Agents
- MCP
---
