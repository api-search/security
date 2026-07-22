---
api_specs:
- filename: rows-openapi.yml
  format: yaml
  label: Rows API
  slug: rows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rows/refs/heads/main/openapi/rows-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:engineering-devops@rows.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: rows.com
  spf: true
hosts:
- cert_expires: Aug 23 20:42:21 2026 GMT
  host: www.rows.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 05:25:54 2026 GMT
  host: api.rows.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rows Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rows, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Rows
provider_slug: rows
slug: rows-domain-security
source_filename: rows-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rows.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 20:42:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.rows.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 05:25:54 2026 GMT\n  hsts: null\ndomains:\n- domain: rows.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:engineering-devops@rows.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rows/refs/heads/main/security/rows-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Productivity
- Spreadsheets
- Data
- No-Code
- Automation
- Artificial Intelligence
- Analytics
- Business Intelligence
---
