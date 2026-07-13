---
api_specs:
- filename: smartsheet-openapi.yml
  format: yaml
  label: Smartsheet REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartsheet/refs/heads/main/openapi/smartsheet-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:security@smartsheet.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: smartsheet.com
  spf: true
hosts:
- cert_expires: Aug 30 18:50:19 2026 GMT
  host: www.smartsheet.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 11 11:15:38 2026 GMT
  host: developers.smartsheet.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: api.smartsheet.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Smartsheet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Smartsheet, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Smartsheet
provider_slug: smartsheet
slug: smartsheet-domain-security
source_filename: smartsheet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.smartsheet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 18:50:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: developers.smartsheet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 11:15:38 2026 GMT\n  hsts: false\n- host: api.smartsheet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: smartsheet.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:security@smartsheet.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smartsheet/refs/heads/main/security/smartsheet-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Work Management
- Project Management
- Collaboration
- Productivity
- Workflow Automation
- Spreadsheets
---
