---
api_specs:
- filename: payerset-openapi.yml
  format: yaml
  label: Payerset Negotiated Rates
  slug: negotiated-rates
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payerset/refs/heads/main/openapi/payerset-openapi.yml
- filename: payerset-openapi.yml
  format: yaml
  label: Payerset Rate Search
  slug: rate-search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payerset/refs/heads/main/openapi/payerset-openapi.yml
- filename: payerset-openapi.yml
  format: yaml
  label: Payerset Datasets
  slug: datasets
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payerset/refs/heads/main/openapi/payerset-openapi.yml
- filename: payerset-openapi.yml
  format: yaml
  label: Payerset Benchmarks
  slug: benchmarks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payerset/refs/heads/main/openapi/payerset-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: payerset.com
  spf: true
hosts:
- cert_expires: Aug 27 18:20:09 2026 GMT
  host: www.payerset.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 15:30:40 2026 GMT
  host: docs.payerset.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.payerset.com
  https: false
kind: domain-security
layout: security
method: probed
name: Payerset Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Payerset, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Payerset
provider_slug: payerset
slug: payerset-domain-security
source_filename: payerset-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.payerset.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 18:20:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.payerset.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 15:30:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.payerset.com\n  https: false\ndomains:\n- domain: payerset.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/payerset/refs/heads/main/security/payerset-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- Price Transparency
- Negotiated Rates
- Machine-Readable Files
- Payer Data
---
