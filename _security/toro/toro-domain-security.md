---
api_specs:
- filename: toro-crews-api-openapi.yml
  format: yaml
  label: Toro Crews API
  slug: toro-crews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toro/refs/heads/main/openapi/toro-crews-api-openapi.yml
- filename: toro-customers-api-openapi.yml
  format: yaml
  label: Toro Customers API
  slug: toro-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toro/refs/heads/main/openapi/toro-customers-api-openapi.yml
- filename: toro-equipment-api-openapi.yml
  format: yaml
  label: Toro Equipment API
  slug: toro-equipment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toro/refs/heads/main/openapi/toro-equipment-api-openapi.yml
- filename: toro-invoices-api-openapi.yml
  format: yaml
  label: Toro Invoices API
  slug: toro-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toro/refs/heads/main/openapi/toro-invoices-api-openapi.yml
- filename: toro-irrigation-api-openapi.yml
  format: yaml
  label: Toro Irrigation API
  slug: toro-irrigation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toro/refs/heads/main/openapi/toro-irrigation-api-openapi.yml
- filename: toro-jobs-api-openapi.yml
  format: yaml
  label: Toro Jobs API
  slug: toro-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toro/refs/heads/main/openapi/toro-jobs-api-openapi.yml
- filename: toro-payments-api-openapi.yml
  format: yaml
  label: Toro Payments API
  slug: toro-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toro/refs/heads/main/openapi/toro-payments-api-openapi.yml
- filename: toro-reports-api-openapi.yml
  format: yaml
  label: Toro Reports API
  slug: toro-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toro/refs/heads/main/openapi/toro-reports-api-openapi.yml
- filename: toro-schedules-api-openapi.yml
  format: yaml
  label: Toro Schedules API
  slug: toro-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toro/refs/heads/main/openapi/toro-schedules-api-openapi.yml
- filename: toro-sensors-api-openapi.yml
  format: yaml
  label: Toro Sensors API
  slug: toro-sensors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toro/refs/heads/main/openapi/toro-sensors-api-openapi.yml
- filename: toro-zones-api-openapi.yml
  format: yaml
  label: Toro Zones API
  slug: toro-zones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toro/refs/heads/main/openapi/toro-zones-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: thetorocompany.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: toro.com
  spf: true
hosts:
- cert_expires: Sep 28 10:25:09 2026 GMT
  host: www.thetorocompany.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 16:46:31 2026 GMT
  host: horizon360.toro.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 23:59:59 2026 GMT
  host: www.toro.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Toro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Toro, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Toro
provider_slug: toro
slug: toro-domain-security
source_filename: toro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.thetorocompany.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 10:25:09 2026 GMT\n  hsts: null\n- host: horizon360.toro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 16:46:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.toro.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 30 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: thetorocompany.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: toro.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/toro/refs/heads/main/security/toro-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Landscaping
- Irrigation
- Golf
- Equipment
- Smart Connected Products
- Fleet Management
- Turf Management
- Fortune 1000
---
