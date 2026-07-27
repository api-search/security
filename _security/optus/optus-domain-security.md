---
api_specs:
- filename: optus-sms-suite-rest-v1-openapi.yml
  format: yaml
  label: Optus SMS Suite REST API v1
  slug: optus-sms-suite-rest-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optus/refs/heads/main/openapi/optus-sms-suite-rest-v1-openapi.yml
- filename: optus-sms-suite-rest-v2-openapi.yml
  format: yaml
  label: Optus SMS Suite SMS Gateway REST API v2
  slug: optus-sms-suite-rest-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optus/refs/heads/main/openapi/optus-sms-suite-rest-v2-openapi.yml
- filename: optus-sms-suite-campaign-manager-openapi.yml
  format: yaml
  label: Optus SMS Suite Campaign Manager API
  slug: optus-sms-suite-campaign-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optus/refs/heads/main/openapi/optus-sms-suite-campaign-manager-openapi.yml
- filename: optus-sms-suite-status-openapi.json
  format: json
  label: Optus SMS Suite Health Monitoring API
  slug: optus-sms-suite-health-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optus/refs/heads/main/openapi/optus-sms-suite-status-openapi.json
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
