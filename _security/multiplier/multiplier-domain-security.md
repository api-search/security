---
api_specs:
- filename: multiplier-openapi.yml
  format: yaml
  label: Multiplier Members API
  slug: members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/multiplier/refs/heads/main/openapi/multiplier-openapi.yml
- filename: multiplier-openapi.yml
  format: yaml
  label: Multiplier Contracts API
  slug: contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/multiplier/refs/heads/main/openapi/multiplier-openapi.yml
- filename: multiplier-openapi.yml
  format: yaml
  label: Multiplier Payroll API
  slug: payroll-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/multiplier/refs/heads/main/openapi/multiplier-openapi.yml
- filename: multiplier-openapi.yml
  format: yaml
  label: Multiplier Payments API
  slug: payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/multiplier/refs/heads/main/openapi/multiplier-openapi.yml
- filename: multiplier-openapi.yml
  format: yaml
  label: Multiplier Time Off API
  slug: time-off-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/multiplier/refs/heads/main/openapi/multiplier-openapi.yml
- filename: multiplier-openapi.yml
  format: yaml
  label: Multiplier Invoices API
  slug: invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/multiplier/refs/heads/main/openapi/multiplier-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "sectigo.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: usemultiplier.com
  spf: true
hosts:
- cert_expires: Aug 20 00:58:46 2026 GMT
  host: www.usemultiplier.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 17:51:20 2026 GMT
  host: help.usemultiplier.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 13:28:45 2026 GMT
  host: api.usemultiplier.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Multiplier Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Multiplier, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Multiplier
provider_slug: multiplier
slug: multiplier-domain-security
source_filename: multiplier-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.usemultiplier.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 00:58:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.usemultiplier.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 17:51:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.usemultiplier.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 13:28:45 2026 GMT\n  hsts: null\ndomains:\n- domain: usemultiplier.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/multiplier/refs/heads/main/security/multiplier-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- EOR
- Global Employment
- Payroll
- HR
- Contractors
---
