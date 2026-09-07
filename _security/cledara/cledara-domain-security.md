---
api_specs:
- filename: cledara-api-openapi.json
  format: json
  label: Cledara API
  slug: cledara-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cledara/refs/heads/main/openapi/cledara-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cledara.com
  spf: true
hosts:
- cert_expires: Nov 27 17:45:19 2026 GMT
  host: www.cledara.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: docs.cledara.com
  https: false
- cert_expires: Jan 28 23:59:59 2027 GMT
  host: api.cledara.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Cledara Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cledara, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cledara
provider_slug: cledara
slug: cledara-domain-security
source_filename: cledara-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cledara.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 17:45:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.cledara.com\n  https: false\n- host: api.cledara.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: cledara.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cledara/refs/heads/main/security/cledara-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Finance
- SaaS Management
- Software Spending
- Spend Management
- Subscription Management
- Virtual Cards
- Expense Management
- FinOps
- MCP
- Market Data
---
