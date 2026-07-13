---
api_specs:
- filename: castoredc-openapi.yml
  format: yaml
  label: Castor Studies API
  slug: castoredc-studies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/castoredc/refs/heads/main/openapi/castoredc-openapi.yml
- filename: castoredc-openapi.yml
  format: yaml
  label: Castor Participants (Records) API
  slug: castoredc-participants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/castoredc/refs/heads/main/openapi/castoredc-openapi.yml
- filename: castoredc-openapi.yml
  format: yaml
  label: Castor Institutes API
  slug: castoredc-institutes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/castoredc/refs/heads/main/openapi/castoredc-openapi.yml
- filename: castoredc-openapi.yml
  format: yaml
  label: Castor Users API
  slug: castoredc-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/castoredc/refs/heads/main/openapi/castoredc-openapi.yml
- filename: castoredc-openapi.yml
  format: yaml
  label: Castor Fields API
  slug: castoredc-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/castoredc/refs/heads/main/openapi/castoredc-openapi.yml
- filename: castoredc-openapi.yml
  format: yaml
  label: Castor Study Data Points API
  slug: castoredc-study-data-points-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/castoredc/refs/heads/main/openapi/castoredc-openapi.yml
- filename: castoredc-openapi.yml
  format: yaml
  label: Castor Reports (Repeating Data) API
  slug: castoredc-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/castoredc/refs/heads/main/openapi/castoredc-openapi.yml
- filename: castoredc-openapi.yml
  format: yaml
  label: Castor Surveys API
  slug: castoredc-surveys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/castoredc/refs/heads/main/openapi/castoredc-openapi.yml
- filename: castoredc-openapi.yml
  format: yaml
  label: Castor Audit Trail API
  slug: castoredc-audit-trail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/castoredc/refs/heads/main/openapi/castoredc-openapi.yml
- filename: castoredc-openapi.yml
  format: yaml
  label: Castor Data Export API
  slug: castoredc-data-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/castoredc/refs/heads/main/openapi/castoredc-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 iodef "mailto:platform-team@castoredc.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: castoredc.com
  spf: true
hosts:
- cert_expires: Aug 19 01:20:08 2026 GMT
  host: www.castoredc.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 23:42:20 2026 GMT
  host: helpdesk.castoredc.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 23:03:40 2026 GMT
  host: data.castoredc.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Castoredc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Castor, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Castor
provider_slug: castoredc
slug: castoredc-domain-security
source_filename: castoredc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.castoredc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 01:20:08 2026 GMT\n  hsts: false\n- host: helpdesk.castoredc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 23:42:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: data.castoredc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 23:03:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: castoredc.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 iodef \"mailto:platform-team@castoredc.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/castoredc/refs/heads/main/security/castoredc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Clinical Trials
- Electronic Data Capture
- EDC
- Clinical Data Management
- Healthcare
- Life Sciences
- Research
---
