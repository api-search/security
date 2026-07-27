---
api_specs:
- filename: propertyme-openapi.json
  format: json
  label: PropertyMe Contacts API
  slug: propertyme-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyme/refs/heads/main/openapi/propertyme-openapi.json
- filename: propertyme-openapi.json
  format: json
  label: PropertyMe Properties API
  slug: propertyme-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyme/refs/heads/main/openapi/propertyme-openapi.json
- filename: propertyme-openapi.json
  format: json
  label: PropertyMe Tenancies API
  slug: propertyme-tenancies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyme/refs/heads/main/openapi/propertyme-openapi.json
- filename: propertyme-openapi.json
  format: json
  label: PropertyMe Inspections API
  slug: propertyme-inspections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyme/refs/heads/main/openapi/propertyme-openapi.json
- filename: propertyme-openapi.json
  format: json
  label: PropertyMe Job Tasks API
  slug: propertyme-job-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyme/refs/heads/main/openapi/propertyme-openapi.json
- filename: propertyme-openapi.json
  format: json
  label: PropertyMe Tasks API
  slug: propertyme-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyme/refs/heads/main/openapi/propertyme-openapi.json
- filename: propertyme-openapi.json
  format: json
  label: PropertyMe Bills API
  slug: propertyme-bills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyme/refs/heads/main/openapi/propertyme-openapi.json
- filename: propertyme-openapi.json
  format: json
  label: PropertyMe Dashboards API
  slug: propertyme-dashboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyme/refs/heads/main/openapi/propertyme-openapi.json
- filename: propertyme-openapi.json
  format: json
  label: PropertyMe Documents and Images API
  slug: propertyme-documents-and-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyme/refs/heads/main/openapi/propertyme-openapi.json
- filename: propertyme-openapi.json
  format: json
  label: PropertyMe Members API
  slug: propertyme-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyme/refs/heads/main/openapi/propertyme-openapi.json
- filename: propertyme-openapi.json
  format: json
  label: PropertyMe Portfolio Connection API
  slug: propertyme-portfolio-connection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/propertyme/refs/heads/main/openapi/propertyme-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: propertyme.com.au
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: propertyme.com
  spf: true
hosts:
- cert_expires: Sep 25 10:32:03 2026 GMT
  host: www.propertyme.com.au
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 04:40:54 2026 GMT
  host: app.propertyme.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Propertyme Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PropertyMe, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: PropertyMe
provider_slug: propertyme
slug: propertyme-domain-security
source_filename: propertyme-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.propertyme.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 10:32:03 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: app.propertyme.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 04:40:54 2026 GMT\n  hsts: null\ndomains:\n- domain: propertyme.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: propertyme.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/propertyme/refs/heads/main/security/propertyme-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real Estate
- Australia
- Property Management
- Rentals
- PropTech
- Tenancy
- Trust Accounting
- Inspections
- Maintenance
- Documents
- Payments
- New Zealand
---
