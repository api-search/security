---
api_specs:
- filename: rjhsignaltech-batch-api-openapi.yml
  format: yaml
  label: Who Represents This Address (RJH Signal Technologies) Batch API
  slug: rjhsignaltech-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rjhsignaltech/refs/heads/main/openapi/rjhsignaltech-batch-api-openapi.yml
- filename: rjhsignaltech-civicinfo-api-openapi.yml
  format: yaml
  label: Who Represents This Address (RJH Signal Technologies) Civicinfo API
  slug: rjhsignaltech-civicinfo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rjhsignaltech/refs/heads/main/openapi/rjhsignaltech-civicinfo-api-openapi.yml
- filename: rjhsignaltech-divisions-api-openapi.yml
  format: yaml
  label: Who Represents This Address (RJH Signal Technologies) Divisions API
  slug: rjhsignaltech-divisions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rjhsignaltech/refs/heads/main/openapi/rjhsignaltech-divisions-api-openapi.yml
- filename: rjhsignaltech-lookup-api-openapi.yml
  format: yaml
  label: Who Represents This Address (RJH Signal Technologies) Lookup API
  slug: rjhsignaltech-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rjhsignaltech/refs/heads/main/openapi/rjhsignaltech-lookup-api-openapi.yml
- filename: rjhsignaltech-x402-api-openapi.yml
  format: yaml
  label: Who Represents This Address (RJH Signal Technologies) X402 API
  slug: rjhsignaltech-x402-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rjhsignaltech/refs/heads/main/openapi/rjhsignaltech-x402-api-openapi.yml
- filename: rjhsignaltech-zip-api-openapi.yml
  format: yaml
  label: Who Represents This Address (RJH Signal Technologies) Zip API
  slug: rjhsignaltech-zip-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rjhsignaltech/refs/heads/main/openapi/rjhsignaltech-zip-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: workers.dev
  spf: true
hosts:
- cert_expires: Dec  1 08:56:50 2026 GMT
  host: whorepresents.rjhsignaltech.workers.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Rjhsignaltech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Who Represents This Address (RJH Signal Technologies), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Who Represents This Address (RJH Signal Technologies)
provider_slug: rjhsignaltech
slug: rjhsignaltech-domain-security
source_filename: rjhsignaltech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: whorepresents.rjhsignaltech.workers.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 08:56:50 2026 GMT\n  hsts: false\ndomains:\n- domain: workers.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rjhsignaltech/refs/heads/main/security/rjhsignaltech-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- API
- Civic
- Government
- Address
---
