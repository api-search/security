---
api_specs:
- filename: unified-to-accounting-openapi.yaml
  format: yaml
  label: Unified.to Accounting API
  slug: accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unified-to/refs/heads/main/openapi/unified-to-accounting-openapi.yaml
- filename: unified-to-marketing-openapi.yaml
  format: yaml
  label: Unified.to Advertising API
  slug: ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unified-to/refs/heads/main/openapi/unified-to-marketing-openapi.yaml
- filename: unified-to-hr-talent-openapi.yaml
  format: yaml
  label: Unified.to Assessment API
  slug: assessment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unified-to/refs/heads/main/openapi/unified-to-hr-talent-openapi.yaml
- filename: unified-to-ats-openapi.yaml
  format: yaml
  label: Unified.to ATS API
  slug: ats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unified-to/refs/heads/main/openapi/unified-to-ats-openapi.yaml
- filename: unified-to-productivity-openapi.yaml
  format: yaml
  label: Unified.to Calendar & Meetings API
  slug: calendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unified-to/refs/heads/main/openapi/unified-to-productivity-openapi.yaml
- filename: unified-to-it-ops-openapi.yaml
  format: yaml
  label: Unified.to Call Center API
  slug: call-center-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unified-to/refs/heads/main/openapi/unified-to-it-ops-openapi.yaml
- filename: unified-to-crm-openapi.yaml
  format: yaml
  label: Unified.to CRM API
  slug: crm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unified-to/refs/heads/main/openapi/unified-to-crm-openapi.yaml
- filename: unified-to-commerce-openapi.yaml
  format: yaml
  label: Unified.to E-Commerce API
  slug: ecommerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unified-to/refs/heads/main/openapi/unified-to-commerce-openapi.yaml
- filename: unified-to-hris-openapi.yaml
  format: yaml
  label: Unified.to HR & Directory API
  slug: hris-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unified-to/refs/heads/main/openapi/unified-to-hris-openapi.yaml
- filename: unified-to-productivity-openapi.yaml
  format: yaml
  label: Unified.to Messaging API
  slug: messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unified-to/refs/heads/main/openapi/unified-to-productivity-openapi.yaml
- filename: unified-to-it-ops-openapi.yaml
  format: yaml
  label: Unified.to Payments API
  slug: payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unified-to/refs/heads/main/openapi/unified-to-it-ops-openapi.yaml
- filename: unified-to-it-ops-openapi.yaml
  format: yaml
  label: Unified.to Ticketing API
  slug: ticketing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unified-to/refs/heads/main/openapi/unified-to-it-ops-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: unified.to
  spf: true
hosts:
- cert_expires: Oct  8 05:28:55 2026 GMT
  host: unified.to
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 23:59:59 2026 GMT
  host: api.unified.to
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  2 23:59:59 2026 GMT
  host: api-eu.unified.to
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Unified To Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Unified.to, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Unified.to
provider_slug: unified-to
slug: unified-to-domain-security
source_filename: unified-to-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: unified.to\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 05:28:55 2026 GMT\n  hsts: false\n- host: api.unified.to\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-eu.unified.to\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: unified.to\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unified-to/refs/heads/main/security/unified-to-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Integrations
- Unified API
---
