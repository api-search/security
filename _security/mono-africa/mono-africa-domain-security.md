---
api_specs:
- filename: mono-africa-openapi.yml
  format: yaml
  label: Mono Connect API
  slug: mono-africa-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mono-africa/refs/heads/main/openapi/mono-africa-openapi.yml
- filename: mono-africa-openapi.yml
  format: yaml
  label: Mono Financial Data API
  slug: mono-africa-financial-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mono-africa/refs/heads/main/openapi/mono-africa-openapi.yml
- filename: mono-africa-openapi.yml
  format: yaml
  label: Mono Investment Data API
  slug: mono-africa-investment-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mono-africa/refs/heads/main/openapi/mono-africa-openapi.yml
- filename: mono-africa-openapi.yml
  format: yaml
  label: Mono Creditworthiness API
  slug: mono-africa-creditworthiness-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mono-africa/refs/heads/main/openapi/mono-africa-openapi.yml
- filename: mono-africa-openapi.yml
  format: yaml
  label: Mono DirectPay API
  slug: mono-africa-directpay-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mono-africa/refs/heads/main/openapi/mono-africa-openapi.yml
- filename: mono-africa-openapi.yml
  format: yaml
  label: Mono Lookup API
  slug: mono-africa-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mono-africa/refs/heads/main/openapi/mono-africa-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mono.co
  spf: true
hosts:
- cert_expires: Dec  9 23:59:59 2026 GMT
  host: mono.co
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 18 23:59:59 2027 GMT
  host: api.withmono.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: docs.mono.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mono Africa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mono, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Mono
provider_slug: mono-africa
slug: mono-africa-domain-security
source_filename: mono-africa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mono.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 23:59:59 2026 GMT\n  hsts: false\n- host: api.withmono.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 18 23:59:59 2027 GMT\n  hsts: false\n- host: docs.mono.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: mono.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mono-africa/refs/heads/main/security/mono-africa-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Open Banking
- Financial Data
- Payments
- Fintech
- Account Linking
- Direct Debit
- Bank Data
- Africa
- Nigeria
- Financial Infrastructure
---
