---
api_specs:
- filename: qgiv-openapi.yml
  format: yaml
  label: Qgiv Transactions API
  slug: qgiv-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qgiv/refs/heads/main/openapi/qgiv-openapi.yml
- filename: qgiv-openapi.yml
  format: yaml
  label: Qgiv Recurring Donations API
  slug: qgiv-recurring-donations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qgiv/refs/heads/main/openapi/qgiv-openapi.yml
- filename: qgiv-openapi.yml
  format: yaml
  label: Qgiv Refunds API
  slug: qgiv-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qgiv/refs/heads/main/openapi/qgiv-openapi.yml
- filename: qgiv-openapi.yml
  format: yaml
  label: Qgiv Peer-to-Peer Registrations API
  slug: qgiv-peer-to-peer-registrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qgiv/refs/heads/main/openapi/qgiv-openapi.yml
- filename: qgiv-openapi.yml
  format: yaml
  label: Qgiv Events API
  slug: qgiv-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qgiv/refs/heads/main/openapi/qgiv-openapi.yml
- filename: qgiv-openapi.yml
  format: yaml
  label: Qgiv Account Settings API
  slug: qgiv-account-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qgiv/refs/heads/main/openapi/qgiv-openapi.yml
- filename: qgiv-openapi.yml
  format: yaml
  label: Qgiv Custom Fields API
  slug: qgiv-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qgiv/refs/heads/main/openapi/qgiv-openapi.yml
- filename: qgiv-openapi.yml
  format: yaml
  label: Qgiv Custom Amounts API
  slug: qgiv-custom-amounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qgiv/refs/heads/main/openapi/qgiv-openapi.yml
- filename: qgiv-openapi.yml
  format: yaml
  label: Qgiv Statements API
  slug: qgiv-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qgiv/refs/heads/main/openapi/qgiv-openapi.yml
- filename: qgiv-openapi.yml
  format: yaml
  label: Qgiv Report Mappings API
  slug: qgiv-report-mappings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qgiv/refs/heads/main/openapi/qgiv-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: qgiv.com
  spf: true
hosts:
- cert_expires: Feb 13 15:46:32 2027 GMT
  host: www.qgiv.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: secure.qgiv.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Qgiv Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Qgiv, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Qgiv
provider_slug: qgiv
slug: qgiv-domain-security
source_filename: qgiv-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.qgiv.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 13 15:46:32 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: secure.qgiv.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: qgiv.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qgiv/refs/heads/main/security/qgiv-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Nonprofit
- Fundraising
- Donations
- Payments
- Peer to Peer
- Events
- Bloomerang
---
