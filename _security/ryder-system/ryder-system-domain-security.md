---
api_specs:
- filename: ryder-system-documents-api-openapi.yml
  format: yaml
  label: Ryder System Documents API
  slug: ryder-system-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ryder-system/refs/heads/main/openapi/ryder-system-documents-api-openapi.yml
- filename: ryder-system-fleet-api-openapi.yml
  format: yaml
  label: Ryder System Fleet API
  slug: ryder-system-fleet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ryder-system/refs/heads/main/openapi/ryder-system-fleet-api-openapi.yml
- filename: ryder-system-invoices-api-openapi.yml
  format: yaml
  label: Ryder System Invoices API
  slug: ryder-system-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ryder-system/refs/heads/main/openapi/ryder-system-invoices-api-openapi.yml
- filename: ryder-system-load-events-api-openapi.yml
  format: yaml
  label: Ryder System Load Events API
  slug: ryder-system-load-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ryder-system/refs/heads/main/openapi/ryder-system-load-events-api-openapi.yml
- filename: ryder-system-loads-api-openapi.yml
  format: yaml
  label: Ryder System Loads API
  slug: ryder-system-loads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ryder-system/refs/heads/main/openapi/ryder-system-loads-api-openapi.yml
- filename: ryder-system-locations-api-openapi.yml
  format: yaml
  label: Ryder System Locations API
  slug: ryder-system-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ryder-system/refs/heads/main/openapi/ryder-system-locations-api-openapi.yml
- filename: ryder-system-service-history-api-openapi.yml
  format: yaml
  label: Ryder System Service History API
  slug: ryder-system-service-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ryder-system/refs/heads/main/openapi/ryder-system-service-history-api-openapi.yml
- filename: ryder-system-ship-confirmation-api-openapi.yml
  format: yaml
  label: Ryder System Ship Confirmation API
  slug: ryder-system-ship-confirmation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ryder-system/refs/heads/main/openapi/ryder-system-ship-confirmation-api-openapi.yml
- filename: ryder-system-ship-status-api-openapi.yml
  format: yaml
  label: Ryder System Ship Status API
  slug: ryder-system-ship-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ryder-system/refs/heads/main/openapi/ryder-system-ship-status-api-openapi.yml
- filename: ryder-system-shipments-api-openapi.yml
  format: yaml
  label: Ryder System Shipments API
  slug: ryder-system-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ryder-system/refs/heads/main/openapi/ryder-system-shipments-api-openapi.yml
- filename: ryder-system-tracking-api-openapi.yml
  format: yaml
  label: Ryder System Tracking API
  slug: ryder-system-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ryder-system/refs/heads/main/openapi/ryder-system-tracking-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ryder.com
  spf: true
hosts:
- cert_expires: Nov 20 23:59:59 2026 GMT
  host: www.ryder.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: developer.ryder.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 20 23:59:59 2026 GMT
  host: api.ryder.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ryder System Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ryder System, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ryder System
provider_slug: ryder-system
slug: ryder-system-domain-security
source_filename: ryder-system-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ryder.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\n- host: developer.ryder.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.ryder.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: ryder.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ryder-system/refs/heads/main/security/ryder-system-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fleet Management
- Logistics
- Supply Chain
- Transportation
- Trucking
- Fortune 500
---
