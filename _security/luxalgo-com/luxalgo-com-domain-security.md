---
api_specs:
- filename: luxalgo-com-library-api-openapi.yml
  format: yaml
  label: LuxAlgo Library API
  slug: luxalgo-com-library-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/luxalgo-com/openapi/luxalgo-com-library-api-openapi.yml
- filename: luxalgo-com-marketing-api-openapi.yml
  format: yaml
  label: LuxAlgo Marketing API
  slug: luxalgo-com-marketing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/luxalgo-com/openapi/luxalgo-com-marketing-api-openapi.yml
- filename: luxalgo-com-payments-api-openapi.yml
  format: yaml
  label: LuxAlgo Payments API
  slug: luxalgo-com-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/luxalgo-com/openapi/luxalgo-com-payments-api-openapi.yml
- filename: luxalgo-com-propfirms-api-openapi.yml
  format: yaml
  label: LuxAlgo Propfirms API
  slug: luxalgo-com-propfirms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/luxalgo-com/openapi/luxalgo-com-propfirms-api-openapi.yml
- filename: luxalgo-com-vela-api-openapi.yml
  format: yaml
  label: LuxAlgo Vela API
  slug: luxalgo-com-vela-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/luxalgo-com/openapi/luxalgo-com-vela-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: luxalgo.com
  spf: true
hosts:
- cert_expires: Jan 17 20:26:09 2027 GMT
  host: luxalgo.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: LuxAlgo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LuxAlgo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: LuxAlgo
provider_slug: luxalgo-com
slug: luxalgo-com-domain-security
source_filename: luxalgo-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: luxalgo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 20:26:09 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: luxalgo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/luxalgo-com/security/luxalgo-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Trading
- Charting
- Finance
- Platform
- Vela
---
