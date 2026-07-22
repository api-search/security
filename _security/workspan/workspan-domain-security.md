---
api_specs:
- filename: workspan-authentication-openapi.yml
  format: yaml
  label: WorkSpan Authentication API
  slug: workspan-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workspan/refs/heads/main/openapi/workspan-authentication-openapi.yml
- filename: workspan-co-sell-openapi.yml
  format: yaml
  label: WorkSpan Co-Sell API
  slug: workspan-co-sell-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workspan/refs/heads/main/openapi/workspan-co-sell-openapi.yml
- filename: workspan-scim-openapi.yml
  format: yaml
  label: WorkSpan SCIM API
  slug: workspan-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workspan/refs/heads/main/openapi/workspan-scim-openapi.yml
- filename: workspan-users-openapi.yml
  format: yaml
  label: WorkSpan Users API
  slug: workspan-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workspan/refs/heads/main/openapi/workspan-users-openapi.yml
- filename: workspan-bulk-openapi.yml
  format: yaml
  label: WorkSpan Bulk API
  slug: workspan-bulk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workspan/refs/heads/main/openapi/workspan-bulk-openapi.yml
- filename: workspan-company-openapi.yml
  format: yaml
  label: WorkSpan Company API
  slug: workspan-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workspan/refs/heads/main/openapi/workspan-company-openapi.yml
- filename: workspan-events-openapi.yml
  format: yaml
  label: WorkSpan Events API
  slug: workspan-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workspan/refs/heads/main/openapi/workspan-events-openapi.yml
- filename: workspan-marketplace-openapi.yml
  format: yaml
  label: WorkSpan Marketplace API
  slug: workspan-marketplace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workspan/refs/heads/main/openapi/workspan-marketplace-openapi.yml
- filename: workspan-object-openapi.yml
  format: yaml
  label: WorkSpan Object API
  slug: workspan-object-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workspan/refs/heads/main/openapi/workspan-object-openapi.yml
- filename: workspan-partner-account-load-openapi.yml
  format: yaml
  label: WorkSpan Partner Account Load API
  slug: workspan-partner-account-load-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workspan/refs/heads/main/openapi/workspan-partner-account-load-openapi.yml
- filename: workspan-report-openapi.yml
  format: yaml
  label: WorkSpan Report API
  slug: workspan-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workspan/refs/heads/main/openapi/workspan-report-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: workspan.com
  spf: true
hosts:
- cert_expires: Sep  9 21:04:52 2026 GMT
  host: www.workspan.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  6 23:59:59 2027 GMT
  host: api-sandbox.workspan.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Workspan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WorkSpan, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: WorkSpan
provider_slug: workspan
slug: workspan-domain-security
source_filename: workspan-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.workspan.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 21:04:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-sandbox.workspan.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  6 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: workspan.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workspan/refs/heads/main/security/workspan-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Co-Sell
- Partnerships
- Ecosystem
- Cloud Marketplaces
- Sales
- B2B
- SaaS
---
