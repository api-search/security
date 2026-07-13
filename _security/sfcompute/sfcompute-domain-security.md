---
api_specs:
- filename: sfcompute-openapi.yml
  format: yaml
  label: SF Compute Orders / Market API
  slug: orders-market
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sfcompute/refs/heads/main/openapi/sfcompute-openapi.yml
- filename: sfcompute-openapi.yml
  format: yaml
  label: SF Compute Contracts API
  slug: contracts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sfcompute/refs/heads/main/openapi/sfcompute-openapi.yml
- filename: sfcompute-openapi.yml
  format: yaml
  label: SF Compute Prices / Quote API
  slug: prices
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sfcompute/refs/heads/main/openapi/sfcompute-openapi.yml
- filename: sfcompute-openapi.yml
  format: yaml
  label: SF Compute Clusters / Nodes API
  slug: clusters-nodes
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sfcompute/refs/heads/main/openapi/sfcompute-openapi.yml
- filename: sfcompute-openapi.yml
  format: yaml
  label: SF Compute Balance API
  slug: balance
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sfcompute/refs/heads/main/openapi/sfcompute-openapi.yml
- filename: sfcompute-openapi.yml
  format: yaml
  label: SF Compute Inference API
  slug: inference
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sfcompute/refs/heads/main/openapi/sfcompute-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sfcompute.com
  spf: true
hosts:
- cert_expires: Aug 26 04:20:16 2026 GMT
  host: sfcompute.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 04:20:16 2026 GMT
  host: docs.sfcompute.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  6 23:59:59 2027 GMT
  host: api.sfcompute.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Sfcompute Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SF Compute, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SF Compute
provider_slug: sfcompute
slug: sfcompute-domain-security
source_filename: sfcompute-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sfcompute.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 04:20:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.sfcompute.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 04:20:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.sfcompute.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  6 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: sfcompute.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sfcompute/refs/heads/main/security/sfcompute-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- GPU
- Compute
- Marketplace
- H100
- Spot Pricing
---
