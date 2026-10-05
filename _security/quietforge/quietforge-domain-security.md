---
api_specs:
- filename: quietforge-convert-api-openapi.yml
  format: yaml
  label: Quietforge Document Conversion API
  slug: document-conversion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quietforge/refs/heads/main/openapi/quietforge-convert-api-openapi.yml
- filename: quietforge-x402-index-api-openapi.yml
  format: yaml
  label: Quietforge x402 Service Index API
  slug: x402-service-index-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quietforge/refs/heads/main/openapi/quietforge-x402-index-api-openapi.yml
- filename: quietforge-sudoku-api-openapi.yml
  format: yaml
  label: Quietforge Puzzle Generation API
  slug: puzzle-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quietforge/refs/heads/main/openapi/quietforge-sudoku-api-openapi.yml
- filename: quietforge-typeset-api-openapi.yml
  format: yaml
  label: Quietforge Book Typesetting API
  slug: book-typesetting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quietforge/refs/heads/main/openapi/quietforge-typeset-api-openapi.yml
- filename: quietforge-familytree-api-openapi.yml
  format: yaml
  label: Quietforge Family Tree Chart API
  slug: family-chart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quietforge/refs/heads/main/openapi/quietforge-familytree-api-openapi.yml
- filename: quietforge-dataset-audit-api-openapi.yml
  format: yaml
  label: Quietforge Dataset Audit API
  slug: dataset-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quietforge/refs/heads/main/openapi/quietforge-dataset-audit-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: pages.dev
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: workers.dev
  spf: true
hosts:
- cert_expires: Dec 21 09:18:18 2026 GMT
  host: quietforge-studio.pages.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 20 02:52:18 2026 GMT
  host: qf-api.quietforge-studio.workers.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Quietforge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quietforge Studio, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Quietforge Studio
provider_slug: quietforge
slug: quietforge-domain-security
source_filename: quietforge-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: quietforge-studio.pages.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 09:18:18 2026 GMT\n  hsts: false\n- host: qf-api.quietforge-studio.workers.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 02:52:18 2026 GMT\n  hsts: false\ndomains:\n- domain: pages.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: workers.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quietforge/refs/heads/main/security/quietforge-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Document Processing
- x402
- Micropayments
- MCP
- pay-per-call
- Cloudflare Workers
- Software-as-a-Service
- Business Automation
---
