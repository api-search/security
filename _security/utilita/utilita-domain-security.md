---
api_specs:
- filename: utilita-components-api-openapi.yml
  format: yaml
  label: Utilita Components API
  slug: utilita-components-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utilita/refs/heads/main/openapi/utilita-components-api-openapi.yml
- filename: utilita-incidents-api-openapi.yml
  format: yaml
  label: Utilita Incidents API
  slug: utilita-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utilita/refs/heads/main/openapi/utilita-incidents-api-openapi.yml
- filename: utilita-scheduled-maintenance-api-openapi.yml
  format: yaml
  label: Utilita Scheduled Maintenance API
  slug: utilita-scheduled-maintenance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utilita/refs/heads/main/openapi/utilita-scheduled-maintenance-api-openapi.yml
- filename: utilita-status-api-openapi.yml
  format: yaml
  label: Utilita Status API
  slug: utilita-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utilita/refs/heads/main/openapi/utilita-status-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: utilita.co.uk
  spf: true
hosts:
- cert_expires: Oct 31 23:59:59 2026 GMT
  host: utilita.co.uk
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 09:22:42 2026 GMT
  host: status.utilita.co.uk
  hsts: true
  hsts_max_age: 259200
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Utilita Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Utilita, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Utilita
provider_slug: utilita
slug: utilita-domain-security
source_filename: utilita-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: utilita.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: status.utilita.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 09:22:42 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\ndomains:\n- domain: utilita.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/utilita/refs/heads/main/security/utilita-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- United Kingdom
- Utilities
- Electricity
- Gas
- Smart Metering
- Prepayment
- Energy Retail
- Status
- Operational Transparency
---
