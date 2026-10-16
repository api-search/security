---
api_specs:
- filename: distyra-authentication-api-openapi.yml
  format: yaml
  label: Brightfield Software Authentication API
  slug: distyra-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/distyra/refs/heads/main/openapi/distyra-authentication-api-openapi.yml
- filename: distyra-billing-api-openapi.yml
  format: yaml
  label: Brightfield Software Billing API
  slug: distyra-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/distyra/refs/heads/main/openapi/distyra-billing-api-openapi.yml
- filename: distyra-catalog-api-openapi.yml
  format: yaml
  label: Brightfield Software Catalog API
  slug: distyra-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/distyra/refs/heads/main/openapi/distyra-catalog-api-openapi.yml
- filename: distyra-connect-api-openapi.yml
  format: yaml
  label: Brightfield Software Connect API
  slug: distyra-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/distyra/refs/heads/main/openapi/distyra-connect-api-openapi.yml
- filename: distyra-enrichment-api-openapi.yml
  format: yaml
  label: Brightfield Software Enrichment API
  slug: distyra-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/distyra/refs/heads/main/openapi/distyra-enrichment-api-openapi.yml
- filename: distyra-feedback-api-openapi.yml
  format: yaml
  label: Brightfield Software Feedback API
  slug: distyra-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/distyra/refs/heads/main/openapi/distyra-feedback-api-openapi.yml
- filename: distyra-system-api-openapi.yml
  format: yaml
  label: Brightfield Software System API
  slug: distyra-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/distyra/refs/heads/main/openapi/distyra-system-api-openapi.yml
- filename: distyra-underwriting-api-openapi.yml
  format: yaml
  label: Brightfield Software Underwriting API
  slug: distyra-underwriting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/distyra/refs/heads/main/openapi/distyra-underwriting-api-openapi.yml
- filename: distyra-webhooks-api-openapi.yml
  format: yaml
  label: Brightfield Software Webhooks API
  slug: distyra-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/distyra/refs/heads/main/openapi/distyra-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: distyra.eu
  spf: true
hosts:
- cert_expires: Nov 25 07:04:46 2026 GMT
  host: distyra.eu
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Distyra Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brightfield Software, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Brightfield Software
provider_slug: distyra
slug: distyra-domain-security
source_filename: distyra-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: distyra.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 07:04:46 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: distyra.eu\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/distyra/refs/heads/main/security/distyra-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Banking
- API
- Fintech
- European
---
