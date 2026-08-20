---
api_specs:
- filename: synchrony-financial-applications-api-openapi.yml
  format: yaml
  label: Synchrony Financial Applications API
  slug: synchrony-financial-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synchrony-financial/refs/heads/main/openapi/synchrony-financial-applications-api-openapi.yml
- filename: synchrony-financial-decisions-api-openapi.yml
  format: yaml
  label: Synchrony Financial Decisions API
  slug: synchrony-financial-decisions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synchrony-financial/refs/heads/main/openapi/synchrony-financial-decisions-api-openapi.yml
- filename: synchrony-financial-payments-api-openapi.yml
  format: yaml
  label: Synchrony Financial Payments API
  slug: synchrony-financial-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synchrony-financial/refs/heads/main/openapi/synchrony-financial-payments-api-openapi.yml
- filename: synchrony-financial-preapprovals-api-openapi.yml
  format: yaml
  label: Synchrony Financial Preapprovals API
  slug: synchrony-financial-preapprovals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synchrony-financial/refs/heads/main/openapi/synchrony-financial-preapprovals-api-openapi.yml
- filename: synchrony-financial-preauthorizations-api-openapi.yml
  format: yaml
  label: Synchrony Financial Preauthorizations API
  slug: synchrony-financial-preauthorizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synchrony-financial/refs/heads/main/openapi/synchrony-financial-preauthorizations-api-openapi.yml
- filename: synchrony-financial-purchases-api-openapi.yml
  format: yaml
  label: Synchrony Financial Purchases API
  slug: synchrony-financial-purchases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synchrony-financial/refs/heads/main/openapi/synchrony-financial-purchases-api-openapi.yml
- filename: synchrony-financial-refunds-api-openapi.yml
  format: yaml
  label: Synchrony Financial Refunds API
  slug: synchrony-financial-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synchrony-financial/refs/heads/main/openapi/synchrony-financial-refunds-api-openapi.yml
- filename: synchrony-financial-reversals-api-openapi.yml
  format: yaml
  label: Synchrony Financial Reversals API
  slug: synchrony-financial-reversals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synchrony-financial/refs/heads/main/openapi/synchrony-financial-reversals-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: synchrony.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: syf.com
  spf: true
hosts:
- cert_expires: Feb  1 23:59:59 2027 GMT
  host: www.synchrony.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: developer.syf.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 28 23:59:59 2026 GMT
  host: api.syf.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Synchrony Financial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Synchrony Financial, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Synchrony Financial
provider_slug: synchrony-financial
slug: synchrony-financial-domain-security
source_filename: synchrony-financial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.synchrony.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.syf.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.syf.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 28 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: synchrony.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: syf.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/synchrony-financial/refs/heads/main/security/synchrony-financial-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Financial-Services
- Credit
- Payments
- Consumer Finance
- Retail Finance
---
