---
api_specs:
- filename: wagepoint-companies-api-openapi.yml
  format: yaml
  label: Wagepoint Companies API
  slug: wagepoint-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wagepoint/refs/heads/main/openapi/wagepoint-companies-api-openapi.yml
- filename: wagepoint-health-api-openapi.yml
  format: yaml
  label: Wagepoint Health API
  slug: wagepoint-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wagepoint/refs/heads/main/openapi/wagepoint-health-api-openapi.yml
- filename: wagepoint-mcp-api-openapi.yml
  format: yaml
  label: Wagepoint MCP API
  slug: wagepoint-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wagepoint/refs/heads/main/openapi/wagepoint-mcp-api-openapi.yml
- filename: wagepoint-pay-groups-api-openapi.yml
  format: yaml
  label: Wagepoint Pay Groups API
  slug: wagepoint-pay-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wagepoint/refs/heads/main/openapi/wagepoint-pay-groups-api-openapi.yml
- filename: wagepoint-persons-api-openapi.yml
  format: yaml
  label: Wagepoint Persons API
  slug: wagepoint-persons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wagepoint/refs/heads/main/openapi/wagepoint-persons-api-openapi.yml
- filename: wagepoint-time-entries-api-openapi.yml
  format: yaml
  label: Wagepoint Time Entries API
  slug: wagepoint-time-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wagepoint/refs/heads/main/openapi/wagepoint-time-entries-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazonaws.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wagepoint.com
  spf: true
hosts:
- cert_expires: Dec 21 23:59:59 2026 GMT
  host: wagepoint.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Wagepoint Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wagepoint, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Wagepoint
provider_slug: wagepoint
slug: wagepoint-domain-security
source_filename: wagepoint-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wagepoint.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: wagepoint.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wagepoint/refs/heads/main/security/wagepoint-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payroll
- Canada
- Software-as-a-Service
- Small Business
---
