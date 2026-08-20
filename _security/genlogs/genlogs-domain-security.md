---
api_specs:
- filename: genlogs-alerts-api-openapi.yml
  format: yaml
  label: GenLogs Alerts API
  slug: genlogs-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genlogs/refs/heads/main/openapi/genlogs-alerts-api-openapi.yml
- filename: genlogs-auth-api-openapi.yml
  format: yaml
  label: GenLogs auth API
  slug: genlogs-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genlogs/refs/heads/main/openapi/genlogs-auth-api-openapi.yml
- filename: genlogs-carrier-api-openapi.yml
  format: yaml
  label: GenLogs Carrier API
  slug: genlogs-carrier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genlogs/refs/heads/main/openapi/genlogs-carrier-api-openapi.yml
- filename: genlogs-carrier-vetting-api-openapi.yml
  format: yaml
  label: GenLogs carrier-vetting API
  slug: genlogs-carrier-vetting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genlogs/refs/heads/main/openapi/genlogs-carrier-vetting-api-openapi.yml
- filename: genlogs-compliance-rules-api-openapi.yml
  format: yaml
  label: GenLogs Compliance Rules API
  slug: genlogs-compliance-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genlogs/refs/heads/main/openapi/genlogs-compliance-rules-api-openapi.yml
- filename: genlogs-facilities-api-openapi.yml
  format: yaml
  label: GenLogs Facilities API
  slug: genlogs-facilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genlogs/refs/heads/main/openapi/genlogs-facilities-api-openapi.yml
- filename: genlogs-mismatch-alerts-api-openapi.yml
  format: yaml
  label: GenLogs Mismatch alerts API
  slug: genlogs-mismatch-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genlogs/refs/heads/main/openapi/genlogs-mismatch-alerts-api-openapi.yml
- filename: genlogs-onboarded-carriers-api-openapi.yml
  format: yaml
  label: GenLogs Onboarded Carriers API
  slug: genlogs-onboarded-carriers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genlogs/refs/heads/main/openapi/genlogs-onboarded-carriers-api-openapi.yml
- filename: genlogs-shipper-api-openapi.yml
  format: yaml
  label: GenLogs Shipper API
  slug: genlogs-shipper-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genlogs/refs/heads/main/openapi/genlogs-shipper-api-openapi.yml
- filename: genlogs-webhook-alerts-api-openapi.yml
  format: yaml
  label: GenLogs Webhook Alerts API
  slug: genlogs-webhook-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genlogs/refs/heads/main/openapi/genlogs-webhook-alerts-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: genlogs.io
  spf: true
hosts:
- cert_expires: Aug 25 00:59:57 2026 GMT
  host: www.genlogs.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 23:59:59 2026 GMT
  host: api.genlogs.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Genlogs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GenLogs, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: GenLogs
provider_slug: genlogs
slug: genlogs-domain-security
source_filename: genlogs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.genlogs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 00:59:57 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.genlogs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: genlogs.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/genlogs/refs/heads/main/security/genlogs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Logistics
- Freight
- Trucking
- Supply Chain
- Carrier Intelligence
- Fleet
- Transportation
- Insurance
- Fraud Detection
- Webhook
- Geospatial
---
