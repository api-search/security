---
api_specs:
- filename: optus-delete-multiple-lists-api-openapi.yml
  format: yaml
  label: Optus Delete Multiple Lists API
  slug: optus-delete-multiple-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optus/refs/heads/main/openapi/optus-delete-multiple-lists-api-openapi.yml
- filename: optus-documentation-api-openapi.yml
  format: yaml
  label: Optus Documentation API
  slug: optus-documentation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optus/refs/heads/main/openapi/optus-documentation-api-openapi.yml
- filename: optus-lists-api-openapi.yml
  format: yaml
  label: Optus Lists API
  slug: optus-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optus/refs/heads/main/openapi/optus-lists-api-openapi.yml
- filename: optus-messages-api-openapi.yml
  format: yaml
  label: Optus Messages API
  slug: optus-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optus/refs/heads/main/openapi/optus-messages-api-openapi.yml
- filename: optus-report-api-openapi.yml
  format: yaml
  label: Optus Report API
  slug: optus-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optus/refs/heads/main/openapi/optus-report-api-openapi.yml
- filename: optus-scheduled-campaigns-api-openapi.yml
  format: yaml
  label: Optus Scheduled Campaigns API
  slug: optus-scheduled-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optus/refs/heads/main/openapi/optus-scheduled-campaigns-api-openapi.yml
- filename: optus-services-api-openapi.yml
  format: yaml
  label: Optus Services API
  slug: optus-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optus/refs/heads/main/openapi/optus-services-api-openapi.yml
- filename: optus-status-api-openapi.yml
  format: yaml
  label: Optus Status API
  slug: optus-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optus/refs/heads/main/openapi/optus-status-api-openapi.yml
- filename: optus-templates-api-openapi.yml
  format: yaml
  label: Optus Templates API
  slug: optus-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optus/refs/heads/main/openapi/optus-templates-api-openapi.yml
description: ''
domains:
- caa:
  - 128 issuewild "entrust.net"
  - 0 issue "globalsign.com"
  - 0 issue "sectigo.com"
  - 0 issue "digicert.com"
  - 0 issuewild "globalsign.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: optus.com.au
  spf: true
hosts:
- cert_expires: Aug  7 23:59:59 2026 GMT
  host: www.optus.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 23:59:59 2026 GMT
  host: sms.optus.com.au
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 23:59:59 2026 GMT
  host: api.sms.optus.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Optus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Optus, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Optus
provider_slug: optus
slug: optus-domain-security
source_filename: optus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.optus.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: sms.optus.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.sms.optus.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: optus.com.au\n  dnssec: false\n  caa:\n  - 128 issuewild \"entrust.net\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/optus/refs/heads/main/security/optus-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Telecommunications
- Australia
- Mobile Network Operator
- Messaging
- SMS
- MMS
- Two-Factor Authentication
- Network APIs
- CAMARA
- Open Gateway
- IoT
- 5G
- Broadband
- Satellite
- Enterprise
---
