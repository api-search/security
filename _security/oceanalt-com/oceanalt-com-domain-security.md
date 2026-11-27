---
api_specs:
- filename: oceanalt-com-free-api-openapi.yml
  format: yaml
  label: OceanAlt Free API
  slug: oceanalt-com-free-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oceanalt-com/openapi/oceanalt-com-free-api-openapi.yml
- filename: oceanalt-com-paid-mpp-api-openapi.yml
  format: yaml
  label: OceanAlt paid (mpp) API
  slug: oceanalt-com-paid-mpp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oceanalt-com/openapi/oceanalt-com-paid-mpp-api-openapi.yml
- filename: oceanalt-com-paid-x402-api-openapi.yml
  format: yaml
  label: OceanAlt paid (x402) API
  slug: oceanalt-com-paid-x402-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oceanalt-com/openapi/oceanalt-com-paid-x402-api-openapi.yml
- filename: oceanalt-com-x402-api-openapi.yml
  format: yaml
  label: OceanAlt X402 API
  slug: oceanalt-com-x402-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oceanalt-com/openapi/oceanalt-com-x402-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: oceanalt.com
  spf: true
hosts:
- cert_expires: Jan  8 22:53:26 2027 GMT
  host: oceanalt.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: OceanAlt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OceanAlt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: OceanAlt
provider_slug: oceanalt-com
slug: oceanalt-com-domain-security
source_filename: oceanalt-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: oceanalt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 22:53:26 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: oceanalt.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/oceanalt-com/security/oceanalt-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Compliance
- Risk Screening
- Investigations
- Developer Tools
---
