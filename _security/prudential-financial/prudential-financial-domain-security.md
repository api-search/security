---
api_specs:
- filename: prudential-financial-developer-api-openapi.yml
  format: yaml
  label: Prudential Financial Developer API
  slug: prudential-financial-developer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prudential-financial/refs/heads/main/openapi/prudential-financial-developer-api-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:pki-support@prudential.com"
  - 0 issue "amazon.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "amazonaws.com"
  - 0 issuewild "globalsign.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: prudential.com
  spf: true
hosts:
- cert_expires: Dec 22 23:59:59 2026 GMT
  host: www.prudential.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 09:21:14 2026 GMT
  host: developers.prudential.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 03:22:34 2026 GMT
  host: developer.apis.prudential.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Prudential Financial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Prudential Financial, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Prudential Financial
provider_slug: prudential-financial
slug: prudential-financial-domain-security
source_filename: prudential-financial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.prudential.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 23:59:59 2026 GMT\n  hsts: false\n- host: developers.prudential.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 09:21:14 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.apis.prudential.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 03:22:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: prudential.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:pki-support@prudential.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issuewild \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prudential-financial/refs/heads/main/security/prudential-financial-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Annuities
- Financial Services
- Insurance
- Retirement
- Fortune 100
---
