---
api_specs:
- filename: kalshispy-com-live-api-key-api-openapi.yml
  format: yaml
  label: KalshiSpy Live (API key) API
  slug: kalshispy-com-live-api-key-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kalshispy-com/openapi/kalshispy-com-live-api-key-api-openapi.yml
- filename: kalshispy-com-market-search-key-optional-api-openapi.yml
  format: yaml
  label: KalshiSpy Market search (key optional) API
  slug: kalshispy-com-market-search-key-optional-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kalshispy-com/openapi/kalshispy-com-market-search-key-optional-api-openapi.yml
- filename: kalshispy-com-public-api-openapi.yml
  format: yaml
  label: KalshiSpy Public API
  slug: kalshispy-com-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kalshispy-com/openapi/kalshispy-com-public-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kalshispy.com
  spf: true
hosts:
- cert_expires: Feb  6 16:01:33 2027 GMT
  host: kalshispy.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: KalshiSpy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KalshiSpy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: KalshiSpy
provider_slug: kalshispy-com
slug: kalshispy-com-domain-security
source_filename: kalshispy-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kalshispy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 16:01:33 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: kalshispy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/kalshispy-com/security/kalshispy-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Analytics
- Finance
- Prediction-Market
- Artificial Intelligence
---
