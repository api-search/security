---
api_specs:
- filename: wm-openapi.yml
  format: yaml
  label: WM Services API
  slug: wm-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wm/refs/heads/main/openapi/wm-openapi.yml
- filename: wm-openapi.yml
  format: yaml
  label: WM Service Operations & Materials API
  slug: wm-service-operations-materials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wm/refs/heads/main/openapi/wm-openapi.yml
- filename: wm-openapi.yml
  format: yaml
  label: WM Service Pricing API
  slug: wm-service-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wm/refs/heads/main/openapi/wm-openapi.yml
- filename: wm-openapi.yml
  format: yaml
  label: WM Invoices & Balance API
  slug: wm-invoices-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wm/refs/heads/main/openapi/wm-openapi.yml
- filename: wm-openapi.yml
  format: yaml
  label: WM Profiles & Preferences API
  slug: wm-profiles-preferences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wm/refs/heads/main/openapi/wm-openapi.yml
- filename: wm-openapi.yml
  format: yaml
  label: WM Contacts API
  slug: wm-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wm/refs/heads/main/openapi/wm-openapi.yml
- filename: wm-openapi.yml
  format: yaml
  label: WM Cases & Tickets API
  slug: wm-cases-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wm/refs/heads/main/openapi/wm-openapi.yml
- filename: wm-openapi.yml
  format: yaml
  label: WM Activities API
  slug: wm-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wm/refs/heads/main/openapi/wm-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wm.com
  spf: true
hosts:
- cert_expires: Aug 24 19:42:41 2026 GMT
  host: www.wm.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: api.wm.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: apitest.wm.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WM, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: WM
provider_slug: wm
slug: wm-domain-security
source_filename: wm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 19:42:41 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.wm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: false\n- host: apitest.wm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: wm.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wm/refs/heads/main/security/wm-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Waste Management
- Recycling
- Environmental Services
- Field Services
- Logistics
- Account Management
- Enterprise
- B2B
---
