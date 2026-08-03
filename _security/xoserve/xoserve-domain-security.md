---
api_specs:
- filename: xoserve-shipper-api-openapi.yml
  format: yaml
  label: Xoserve Shipper API
  slug: xoserve-shipper-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xoserve/refs/heads/main/openapi/xoserve-shipper-api-openapi.yml
- filename: xoserve-supplier-api-openapi.yml
  format: yaml
  label: Xoserve Supplier API
  slug: xoserve-supplier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xoserve/refs/heads/main/openapi/xoserve-supplier-api-openapi.yml
- filename: xoserve-meter-asset-api-v1-openapi.yml
  format: yaml
  label: Xoserve Meter Asset (Xoserve Meter Asset Api V1)
  slug: xoserve-meter-asset-api-v1-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xoserve/refs/heads/main/openapi/xoserve-meter-asset-api-v1-openapi.yml
- filename: xoserve-meter-asset-api-v2-openapi.yml
  format: yaml
  label: Xoserve Meter Asset (Xoserve Meter Asset Api V2)
  slug: xoserve-meter-asset-api-v2-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xoserve/refs/heads/main/openapi/xoserve-meter-asset-api-v2-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: xoserve.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: correla.com
  spf: true
hosts:
- cert_expires: Jan 30 23:59:59 2027 GMT
  host: www.xoserve.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 15:31:58 2026 GMT
  host: discoveryapiportal.correla.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct  5 15:31:42 2026 GMT
  host: discoveryapi.correla.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Xoserve Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Xoserve, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Xoserve
provider_slug: xoserve
slug: xoserve-domain-security
source_filename: xoserve-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.xoserve.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: discoveryapiportal.correla.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  5 15:31:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: discoveryapi.correla.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  5 15:31:42 2026 GMT\n  hsts: null\ndomains:\n- domain: xoserve.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: correla.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xoserve/refs/heads/main/security/xoserve-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- United Kingdom
- Gas
- Utilities
- Energy Markets
- Meter Data
- Gas Networks
- Central Data Service Provider
- Data Services
---
