---
api_specs:
- filename: cariqa-billing-details-api-openapi.yml
  format: yaml
  label: Cariqa Billing Details API
  slug: cariqa-billing-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cariqa/refs/heads/main/openapi/cariqa-billing-details-api-openapi.yml
- filename: cariqa-charging-sessions-api-openapi.yml
  format: yaml
  label: Cariqa Charging Sessions API
  slug: cariqa-charging-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cariqa/refs/heads/main/openapi/cariqa-charging-sessions-api-openapi.yml
- filename: cariqa-debts-api-openapi.yml
  format: yaml
  label: Cariqa Debts API
  slug: cariqa-debts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cariqa/refs/heads/main/openapi/cariqa-debts-api-openapi.yml
- filename: cariqa-invoices-api-openapi.yml
  format: yaml
  label: Cariqa Invoices API
  slug: cariqa-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cariqa/refs/heads/main/openapi/cariqa-invoices-api-openapi.yml
- filename: cariqa-payments-api-openapi.yml
  format: yaml
  label: Cariqa Payments API
  slug: cariqa-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cariqa/refs/heads/main/openapi/cariqa-payments-api-openapi.yml
- filename: cariqa-stations-api-openapi.yml
  format: yaml
  label: Cariqa Stations API
  slug: cariqa-stations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cariqa/refs/heads/main/openapi/cariqa-stations-api-openapi.yml
- filename: cariqa-users-api-openapi.yml
  format: yaml
  label: Cariqa Users API
  slug: cariqa-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cariqa/refs/heads/main/openapi/cariqa-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: cariqa.com
  spf: true
hosts:
- cert_expires: Sep 10 03:53:27 2026 GMT
  host: cariqa.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 17:20:28 2026 GMT
  host: connect.cariqa.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 10:39:54 2026 GMT
  host: dev.connect.cariqa.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cariqa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cariqa, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Cariqa
provider_slug: cariqa
slug: cariqa-domain-security
source_filename: cariqa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cariqa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 03:53:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: connect.cariqa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 17:20:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dev.connect.cariqa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 10:39:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cariqa.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cariqa/refs/heads/main/security/cariqa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- EV Charging
- Electric Vehicles
- Payments
- Mobility
- e-Mobility
- Charge Point Operator
- Energy
---
