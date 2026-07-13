---
api_specs:
- filename: bny-mellon-treasury-services-api-openapi.yml
  format: yaml
  label: BNY Mellon Treasury Services API
  slug: treasury-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-new-york-mellon/refs/heads/main/openapi/bny-mellon-treasury-services-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bnymellon.com
  spf: true
hosts:
- cert_expires: Sep 28 23:59:59 2026 GMT
  host: www.bnymellon.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 14 23:59:59 2027 GMT
  host: marketplace.bnymellon.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- host: api.bnymellon.com
  https: false
kind: domain-security
layout: security
method: probed
name: Bank Of New York Mellon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BNY Mellon, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: BNY Mellon
provider_slug: bank-of-new-york-mellon
slug: bank-of-new-york-mellon-domain-security
source_filename: bank-of-new-york-mellon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bnymellon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\n- host: marketplace.bnymellon.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 14 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.bnymellon.com\n  https: false\ndomains:\n- domain: bnymellon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bank-of-new-york-mellon/refs/heads/main/security/bank-of-new-york-mellon-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Asset Servicing
- Banking
- Institutional Banking
- Payments
- Treasury
- Wire Transfers
- Fortune 500
---
