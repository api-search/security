---
api_specs:
- filename: measurabl-core-openapi.yml
  format: yaml
  label: Measurabl Core API
  slug: measurabl-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/measurabl/refs/heads/main/openapi/measurabl-core-openapi.yml
- filename: measurabl-esgx-buildings-openapi.yml
  format: yaml
  label: Measurabl ESGx Buildings API
  slug: measurabl-esgx-buildings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/measurabl/refs/heads/main/openapi/measurabl-esgx-buildings-openapi.yml
- filename: measurabl-esgx-securities-openapi.yml
  format: yaml
  label: Measurabl ESGx Securities API
  slug: measurabl-esgx-securities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/measurabl/refs/heads/main/openapi/measurabl-esgx-securities-openapi.yml
- filename: measurabl-esgx-securities-compliance-files-openapi.yml
  format: yaml
  label: Measurabl ESGx Securities Compliance Files API
  slug: measurabl-esgx-securities-compliance-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/measurabl/refs/heads/main/openapi/measurabl-esgx-securities-compliance-files-openapi.yml
- filename: measurabl-partners-openapi.yml
  format: yaml
  label: Measurabl Partner API
  slug: measurabl-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/measurabl/refs/heads/main/openapi/measurabl-partners-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: measurabl.com
  spf: true
hosts:
- cert_expires: Sep  3 22:24:26 2026 GMT
  host: www.measurabl.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 28 23:59:59 2027 GMT
  host: api.measurabl.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Measurabl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Measurabl, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Measurabl
provider_slug: measurabl
slug: measurabl-domain-security
source_filename: measurabl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.measurabl.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 22:24:26 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.measurabl.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 28 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: measurabl.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/measurabl/refs/heads/main/security/measurabl-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- ESG
- Real-Estate
- Sustainability
- Carbon Accounting
- Energy Management
- Building Performance
- Climate Risk
- Benchmarking
- Compliance
- PropTech
- Utility Data
- Capital Markets
---
