---
api_specs:
- filename: spreadshirt-spreadconnect-openapi.json
  format: json
  label: SpreadConnect (SPOD) Fulfillment API
  slug: spreadconnect-spod-fulfillment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spreadshirt/refs/heads/main/openapi/spreadshirt-spreadconnect-openapi.json
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  dmarc: false
  dnssec: true
  domain: spreadshirt.com
  spf: true
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: spreadconnect.app
  spf: true
hosts:
- cert_expires: Oct 15 16:28:07 2026 GMT
  host: www.spreadshirt.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 13:28:12 2026 GMT
  host: api.spreadconnect.app
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 15:33:35 2026 GMT
  host: developer.spreadshirt.net
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spreadshirt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spreadshirt, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Spreadshirt
provider_slug: spreadshirt
slug: spreadshirt-domain-security
source_filename: spreadshirt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.spreadshirt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 16:28:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.spreadconnect.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 13:28:12 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: developer.spreadshirt.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 15:33:35 2026 GMT\n  hsts: false\ndomains:\n- domain: spreadshirt.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: false\n- domain: spreadconnect.app\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spreadshirt/refs/heads/main/security/spreadshirt-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Consumer
- Print on Demand
- E-commerce
- Apparel
- Custom Merchandise
- Fulfillment
- Dropshipping
- Webhooks
---
