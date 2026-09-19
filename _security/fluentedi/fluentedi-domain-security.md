---
api_specs:
- filename: fluentedi-compute-api-openapi.yml
  format: yaml
  label: FluentEDI Compute API
  slug: fluentedi-compute-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fluentedi/refs/heads/main/openapi/fluentedi-compute-api-openapi.yml
- filename: fluentedi-crypto-api-openapi.yml
  format: yaml
  label: FluentEDI Crypto API
  slug: fluentedi-crypto-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fluentedi/refs/heads/main/openapi/fluentedi-crypto-api-openapi.yml
- filename: fluentedi-data-api-openapi.yml
  format: yaml
  label: FluentEDI Data API
  slug: fluentedi-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fluentedi/refs/heads/main/openapi/fluentedi-data-api-openapi.yml
- filename: fluentedi-doc-api-openapi.yml
  format: yaml
  label: FluentEDI Doc API
  slug: fluentedi-doc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fluentedi/refs/heads/main/openapi/fluentedi-doc-api-openapi.yml
- filename: fluentedi-edi-api-openapi.yml
  format: yaml
  label: FluentEDI Edi API
  slug: fluentedi-edi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fluentedi/refs/heads/main/openapi/fluentedi-edi-api-openapi.yml
- filename: fluentedi-meta-api-openapi.yml
  format: yaml
  label: FluentEDI Meta API
  slug: fluentedi-meta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fluentedi/refs/heads/main/openapi/fluentedi-meta-api-openapi.yml
- filename: fluentedi-schedule-api-openapi.yml
  format: yaml
  label: FluentEDI Schedule API
  slug: fluentedi-schedule-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fluentedi/refs/heads/main/openapi/fluentedi-schedule-api-openapi.yml
- filename: fluentedi-text-api-openapi.yml
  format: yaml
  label: FluentEDI Text API
  slug: fluentedi-text-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fluentedi/refs/heads/main/openapi/fluentedi-text-api-openapi.yml
- filename: fluentedi-time-api-openapi.yml
  format: yaml
  label: FluentEDI Time API
  slug: fluentedi-time-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fluentedi/refs/heads/main/openapi/fluentedi-time-api-openapi.yml
- filename: fluentedi-web-api-openapi.yml
  format: yaml
  label: FluentEDI Web API
  slug: fluentedi-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fluentedi/refs/heads/main/openapi/fluentedi-web-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: fluentedi.com
  spf: false
hosts:
- cert_expires: Oct 17 16:51:25 2026 GMT
  host: fluentedi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fluentedi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FluentEDI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: FluentEDI
provider_slug: fluentedi
slug: fluentedi-domain-security
source_filename: fluentedi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fluentedi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 16:51:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fluentedi.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fluentedi/refs/heads/main/security/fluentedi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- EDI
- X12
- Retail EDI
- AI Agents
- MCP
- Developer Tools
- JSON
- Cryptography
- Data Validation
- Supply Chain
---
