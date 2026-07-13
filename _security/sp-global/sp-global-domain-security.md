---
api_specs:
- filename: kensho-llmready-openapi.yml
  format: yaml
  label: S&P Global LLM-Ready API (kFinance)
  slug: kensho-llm-ready-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sp-global/refs/heads/main/openapi/kensho-llmready-openapi.yml
- filename: kensho-extract-openapi.yml
  format: yaml
  label: Kensho Extract API
  slug: kensho-extract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sp-global/refs/heads/main/openapi/kensho-extract-openapi.yml
- filename: kensho-nerd-openapi.yml
  format: yaml
  label: Kensho NERD API
  slug: kensho-nerd-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sp-global/refs/heads/main/openapi/kensho-nerd-openapi.yml
- filename: kensho-scribe-batch-v2-openapi.yml
  format: yaml
  label: Kensho Scribe Batch API v2
  slug: kensho-scribe-batch-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sp-global/refs/heads/main/openapi/kensho-scribe-batch-v2-openapi.yml
- filename: kensho-scribe-realtime-asyncapi.yml
  format: yaml
  label: Kensho Scribe Real Time API
  slug: kensho-scribe-realtime-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/sp-global/refs/heads/main/asyncapi/kensho-scribe-realtime-asyncapi.yml
- filename: kensho-scribe-batch-v1-openapi.yml
  format: yaml
  label: Kensho Scribe Batch API v1
  slug: kensho-scribe-batch-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sp-global/refs/heads/main/openapi/kensho-scribe-batch-v1-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: spglobal.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kensho.com
  spf: true
hosts:
- cert_expires: Mar  4 23:59:59 2027 GMT
  host: developer.spglobal.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 12 23:59:59 2026 GMT
  host: docs.kensho.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 12 23:59:59 2026 GMT
  host: kfinance.kensho.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sp Global Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for S&P Global, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: S&P Global
provider_slug: sp-global
slug: sp-global-domain-security
source_filename: sp-global-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.spglobal.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  4 23:59:59 2027 GMT\n  hsts: false\n- host: docs.kensho.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\n- host: kfinance.kensho.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: spglobal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: kensho.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sp-global/refs/heads/main/security/sp-global-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Capital IQ
- Commodity Insights
- Credit Ratings
- Document Extraction
- ESG
- Financial Data
- Index Data
- LLM
- MCP
- Market Intelligence
- Mobility
- Named Entity Recognition
- Speech to Text
---
