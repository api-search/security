---
api_specs:
- filename: ramp-developer-api-openapi.yml
  format: yaml
  label: Ramp Developer API
  slug: ramp-developer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ramp/refs/heads/main/openapi/ramp-developer-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ramp.com
  spf: true
hosts:
- cert_expires: Oct  6 03:30:50 2026 GMT
  host: ramp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 22:20:50 2026 GMT
  host: docs.ramp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 03:30:50 2026 GMT
  host: api.ramp.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ramp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ramp, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Ramp
provider_slug: ramp
slug: ramp-domain-security
source_filename: ramp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ramp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 03:30:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.ramp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 22:20:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.ramp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 03:30:50 2026 GMT\n  hsts: null\ndomains:\n- domain: ramp.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ramp/refs/heads/main/security/ramp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Finance
- Spend Management
- Corporate Cards
- Expense Management
- Accounts Payable
- Bill Pay
- Accounting
- Reimbursements
---
