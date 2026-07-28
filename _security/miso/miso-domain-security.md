---
api_specs:
- filename: miso-public-api-operations-displays-openapi.json
  format: json
  label: MISO Public API - Operations Displays
  slug: miso-public-api-operations-displays
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/miso/refs/heads/main/openapi/miso-public-api-operations-displays-openapi.json
- filename: miso-public-api-markets-displays-openapi.json
  format: json
  label: MISO Public API - Markets Displays
  slug: miso-public-api-markets-displays
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/miso/refs/heads/main/openapi/miso-public-api-markets-displays-openapi.json
- filename: miso-data-exchange-pricing-api-openapi.json
  format: json
  label: MISO Data Exchange Pricing API
  slug: miso-data-exchange-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/miso/refs/heads/main/openapi/miso-data-exchange-pricing-api-openapi.json
- filename: miso-data-exchange-load-generation-interchange-api-openapi.json
  format: json
  label: MISO Data Exchange Load, Generation, and Interchange API
  slug: miso-data-exchange-load-generation-interchange-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/miso/refs/heads/main/openapi/miso-data-exchange-load-generation-interchange-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: misoenergy.org
  spf: true
hosts:
- cert_expires: Apr 14 13:41:08 2027 GMT
  host: www.misoenergy.org
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  8 23:59:59 2026 GMT
  host: public-api.misoenergy.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  1 15:51:06 2026 GMT
  host: data-exchange.misoenergy.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Miso Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MISO, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: MISO
provider_slug: miso
slug: miso-domain-security
source_filename: miso-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.misoenergy.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 14 13:41:08 2027 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: public-api.misoenergy.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: false\n- host: data-exchange.misoenergy.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 15:51:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: misoenergy.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/miso/refs/heads/main/security/miso-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- United States
- Electricity
- Energy Markets
- Grid
- System Operator
- Market Operator
- Wholesale Power
- Open Energy Data
- Renewables
- Solar
- Demand Response
- Utilities
---
