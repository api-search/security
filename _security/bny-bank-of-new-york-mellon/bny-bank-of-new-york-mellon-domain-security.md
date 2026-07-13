---
api_specs:
- filename: bny-asset-servicing-api-openapi.yml
  format: yaml
  label: BNY Asset Servicing API
  slug: asset-servicing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bny-bank-of-new-york-mellon/refs/heads/main/openapi/bny-asset-servicing-api-openapi.yml
- filename: bny-treasury-services-api-openapi.yml
  format: yaml
  label: BNY Treasury Services API
  slug: treasury-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bny-bank-of-new-york-mellon/refs/heads/main/openapi/bny-treasury-services-api-openapi.yml
- filename: bny-pershing-api-openapi.yml
  format: yaml
  label: BNY Pershing API
  slug: pershing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bny-bank-of-new-york-mellon/refs/heads/main/openapi/bny-pershing-api-openapi.yml
- filename: bny-markets-api-openapi.yml
  format: yaml
  label: BNY Markets API
  slug: markets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bny-bank-of-new-york-mellon/refs/heads/main/openapi/bny-markets-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bny.com
  spf: true
hosts:
- cert_expires: Sep 16 23:59:59 2026 GMT
  host: www.bny.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 20 23:59:59 2026 GMT
  host: developer.bny.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 14 23:59:59 2027 GMT
  host: apigateway.bny.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Bny Bank Of New York Mellon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BNY (Bank of New York Mellon), probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: BNY (Bank of New York Mellon)
provider_slug: bny-bank-of-new-york-mellon
slug: bny-bank-of-new-york-mellon-domain-security
source_filename: bny-bank-of-new-york-mellon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bny.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\n- host: developer.bny.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apigateway.bny.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 14 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: bny.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bny-bank-of-new-york-mellon/refs/heads/main/security/bny-bank-of-new-york-mellon-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Banking
- Custody
- Asset Servicing
- Treasury Services
- Payments
- Wealth Management
- Clearing
- Capital Markets
- Digital Assets
- Financial Services
---
