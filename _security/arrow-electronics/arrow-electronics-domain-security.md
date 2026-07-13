---
api_specs:
- filename: arrow-electronics-openapi.yml
  format: yaml
  label: Arrow Electronics Pricing and Availability API
  slug: pricing-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arrow-electronics/refs/heads/main/openapi/arrow-electronics-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: arrow.com
  spf: true
hosts:
- cert_expires: Nov  8 23:59:59 2026 GMT
  host: developers.arrow.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 14 23:59:59 2026 GMT
  host: www.arrow.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: api.arrow.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Arrow Electronics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arrow Electronics, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Arrow Electronics
provider_slug: arrow-electronics
slug: arrow-electronics-domain-security
source_filename: arrow-electronics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.arrow.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  8 23:59:59 2026 GMT\n  hsts: false\n- host: www.arrow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:59:59 2026 GMT\n  hsts: null\n- host: api.arrow.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: arrow.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arrow-electronics/refs/heads/main/security/arrow-electronics-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Electronics
- Components
- Supply Chain
- Procurement
- Distribution
- Fortune 500
---
