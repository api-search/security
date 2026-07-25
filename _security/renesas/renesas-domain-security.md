---
api_specs:
- filename: renesas-board-kit-api-openapi.yml
  format: yaml
  label: Renesas Board & Kit API
  slug: renesas-board-kit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/renesas/refs/heads/main/openapi/renesas-board-kit-api-openapi.yml
- filename: renesas-document-api-openapi.yml
  format: yaml
  label: Renesas Document API
  slug: renesas-document-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/renesas/refs/heads/main/openapi/renesas-document-api-openapi.yml
- filename: renesas-package-api-openapi.yml
  format: yaml
  label: Renesas Package API
  slug: renesas-package-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/renesas/refs/heads/main/openapi/renesas-package-api-openapi.yml
- filename: renesas-product-api-openapi.yml
  format: yaml
  label: Renesas Product API
  slug: renesas-product-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/renesas/refs/heads/main/openapi/renesas-product-api-openapi.yml
- filename: renesas-product-part-api-openapi.yml
  format: yaml
  label: Renesas Product Part API
  slug: renesas-product-part-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/renesas/refs/heads/main/openapi/renesas-product-part-api-openapi.yml
- filename: renesas-software-tool-api-openapi.yml
  format: yaml
  label: Renesas Software Tool API
  slug: renesas-software-tool-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/renesas/refs/heads/main/openapi/renesas-software-tool-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: renesas.com
  spf: true
hosts:
- cert_expires: Aug 30 08:45:45 2026 GMT
  host: www.renesas.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 06:44:55 2026 GMT
  host: developer.renesas.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 16:56:17 2026 GMT
  host: api.renesas.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Renesas Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Renesas, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Renesas
provider_slug: renesas
slug: renesas-domain-security
source_filename: renesas-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.renesas.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 08:45:45 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: developer.renesas.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 06:44:55 2026 GMT\n  hsts: false\n- host: api.renesas.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 16:56:17 2026 GMT\n  hsts: null\ndomains:\n- domain: renesas.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/renesas/refs/heads/main/security/renesas-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Semiconductors
- Microcontrollers
- Electronics
- Hardware
- Product Data
- Developer Portal
- Automotive
- Industrial
- Embedded
---
