---
api_specs:
- filename: nirvana-openapi.yml
  format: yaml
  label: Nirvana Eligibility & Coverage API
  slug: eligibility-coverage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nirvana/refs/heads/main/openapi/nirvana-openapi.yml
- filename: nirvana-openapi.yml
  format: yaml
  label: Nirvana Coverage Scan API
  slug: coverage-scan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nirvana/refs/heads/main/openapi/nirvana-openapi.yml
- filename: nirvana-openapi.yml
  format: yaml
  label: Nirvana Benefits API
  slug: benefits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nirvana/refs/heads/main/openapi/nirvana-openapi.yml
- filename: nirvana-openapi.yml
  format: yaml
  label: Nirvana Cost Estimation API
  slug: cost-estimation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nirvana/refs/heads/main/openapi/nirvana-openapi.yml
- filename: nirvana-openapi.yml
  format: yaml
  label: Nirvana Medicaid API
  slug: medicaid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nirvana/refs/heads/main/openapi/nirvana-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: readme.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: meetnirvana.com
  spf: true
hosts:
- cert_expires: Oct  9 13:12:37 2026 GMT
  host: nirvana-docs.readme.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 29 23:59:59 2026 GMT
  host: coverage-api.meetnirvana.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nirvana Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nirvana Health, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Nirvana Health
provider_slug: nirvana
slug: nirvana-domain-security
source_filename: nirvana-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nirvana-docs.readme.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 13:12:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: coverage-api.meetnirvana.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: readme.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: meetnirvana.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nirvana/refs/heads/main/security/nirvana-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- Insurance
- Eligibility
- Benefits
- Cost Estimation
- Behavioral Health
---
