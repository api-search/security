---
api_specs:
- filename: vantage-cost-management-api-openapi.yml
  format: yaml
  label: Vantage Cost Management API
  slug: cost-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vantage/refs/heads/main/openapi/vantage-cost-management-api-openapi.yml
- filename: vantage-cloud-pricing-api-openapi.yml
  format: yaml
  label: Vantage Cloud Pricing API
  slug: cloud-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vantage/refs/heads/main/openapi/vantage-cloud-pricing-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vantage.sh
  spf: true
hosts:
- cert_expires: Oct  2 16:33:05 2026 GMT
  host: docs.vantage.sh
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 29 23:59:59 2026 GMT
  host: api.vantage.sh
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vantage Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vantage, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Vantage
provider_slug: vantage
slug: vantage-domain-security
source_filename: vantage-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.vantage.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 16:33:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.vantage.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: vantage.sh\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vantage/refs/heads/main/security/vantage-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Budgets
- Cloud Pricing
- Cost Management
- Costs
- FinOps
---
