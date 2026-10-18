---
api_specs:
- filename: precoro-invoices-api-openapi.yml
  format: yaml
  label: Precoro Invoices API
  slug: precoro-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/precoro/refs/heads/main/openapi/precoro-invoices-api-openapi.yml
- filename: precoro-items-api-openapi.yml
  format: yaml
  label: Precoro Items API
  slug: precoro-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/precoro/refs/heads/main/openapi/precoro-items-api-openapi.yml
- filename: precoro-legalentities-api-openapi.yml
  format: yaml
  label: Precoro Legalentities API
  slug: precoro-legalentities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/precoro/refs/heads/main/openapi/precoro-legalentities-api-openapi.yml
- filename: precoro-locations-api-openapi.yml
  format: yaml
  label: Precoro Locations API
  slug: precoro-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/precoro/refs/heads/main/openapi/precoro-locations-api-openapi.yml
- filename: precoro-purchaseorders-api-openapi.yml
  format: yaml
  label: Precoro Purchaseorders API
  slug: precoro-purchaseorders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/precoro/refs/heads/main/openapi/precoro-purchaseorders-api-openapi.yml
- filename: precoro-purchaserequisitions-api-openapi.yml
  format: yaml
  label: Precoro Purchaserequisitions API
  slug: precoro-purchaserequisitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/precoro/refs/heads/main/openapi/precoro-purchaserequisitions-api-openapi.yml
- filename: precoro-receipts-api-openapi.yml
  format: yaml
  label: Precoro Receipts API
  slug: precoro-receipts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/precoro/refs/heads/main/openapi/precoro-receipts-api-openapi.yml
- filename: precoro-suppliers-api-openapi.yml
  format: yaml
  label: Precoro Suppliers API
  slug: precoro-suppliers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/precoro/refs/heads/main/openapi/precoro-suppliers-api-openapi.yml
- filename: precoro-taxes-api-openapi.yml
  format: yaml
  label: Precoro Taxes API
  slug: precoro-taxes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/precoro/refs/heads/main/openapi/precoro-taxes-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: precoro.com
  spf: true
hosts:
- cert_expires: Dec 25 23:47:20 2026 GMT
  host: www.precoro.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Precoro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Precoro, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Precoro
provider_slug: precoro
slug: precoro-domain-security
source_filename: precoro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.precoro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:47:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: precoro.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/precoro/refs/heads/main/security/precoro-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Procurement
- Spend Management
- Vendor Management
- Purchase-To-Pay
- AP Automation
- Contract Management
- AI Procurement
---
