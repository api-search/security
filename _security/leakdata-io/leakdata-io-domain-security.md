---
api_specs:
- filename: leakdata-io-alerts-api-openapi.yml
  format: yaml
  label: LeakData Alerts API
  slug: leakdata-io-alerts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leakdata-io/openapi/leakdata-io-alerts-api-openapi.yml
- filename: leakdata-io-domains-api-openapi.yml
  format: yaml
  label: LeakData Domains API
  slug: leakdata-io-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leakdata-io/openapi/leakdata-io-domains-api-openapi.yml
- filename: leakdata-io-easm-api-openapi.yml
  format: yaml
  label: LeakData EASM API
  slug: leakdata-io-easm-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leakdata-io/openapi/leakdata-io-easm-api-openapi.yml
- filename: leakdata-io-password-api-openapi.yml
  format: yaml
  label: LeakData Password API
  slug: leakdata-io-password-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leakdata-io/openapi/leakdata-io-password-api-openapi.yml
- filename: leakdata-io-search-api-openapi.yml
  format: yaml
  label: LeakData Search API
  slug: leakdata-io-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leakdata-io/openapi/leakdata-io-search-api-openapi.yml
- filename: leakdata-io-social-api-openapi.yml
  format: yaml
  label: LeakData Social API
  slug: leakdata-io-social-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leakdata-io/openapi/leakdata-io-social-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: leakdata.io
  spf: true
hosts:
- cert_expires: Dec 22 00:33:03 2026 GMT
  host: leakdata.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: LeakData Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LeakData, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: LeakData
provider_slug: leakdata-io
slug: leakdata-io-domain-security
source_filename: leakdata-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: leakdata.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 00:33:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: leakdata.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/leakdata-io/security/leakdata-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Data Breaches
- Digital Risk
- Cybersecurity
- Monitoring
- Intelligence
---
