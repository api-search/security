---
api_specs:
- filename: minoa-io-company-api-openapi.yml
  format: yaml
  label: Minoa Company API
  slug: minoa-io-company-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/minoa-io/openapi/minoa-io-company-api-openapi.yml
- filename: minoa-io-content-api-openapi.yml
  format: yaml
  label: Minoa Content API
  slug: minoa-io-content-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/minoa-io/openapi/minoa-io-content-api-openapi.yml
- filename: minoa-io-discovery-api-openapi.yml
  format: yaml
  label: Minoa Discovery API
  slug: minoa-io-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/minoa-io/openapi/minoa-io-discovery-api-openapi.yml
- filename: minoa-io-forms-api-openapi.yml
  format: yaml
  label: Minoa Forms API
  slug: minoa-io-forms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/minoa-io/openapi/minoa-io-forms-api-openapi.yml
- filename: minoa-io-pricing-api-openapi.yml
  format: yaml
  label: Minoa Pricing API
  slug: minoa-io-pricing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/minoa-io/openapi/minoa-io-pricing-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: minoa.io
  spf: true
hosts:
- cert_expires: Jan 11 05:34:47 2027 GMT
  host: minoa.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Minoa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Minoa, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Minoa
provider_slug: minoa-io
slug: minoa-io-domain-security
source_filename: minoa-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: minoa.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 05:34:47 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: minoa.io\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/minoa-io/security/minoa-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Value-Intelligence
- Software-as-a-Service
- B2B
- Analytics
---
