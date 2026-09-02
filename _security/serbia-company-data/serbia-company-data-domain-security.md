---
api_specs:
- filename: serbia-company-data-company-api-openapi.yml
  format: yaml
  label: Serbia Company Data Company API
  slug: serbia-company-data-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serbia-company-data/refs/heads/main/openapi/serbia-company-data-company-api-openapi.yml
- filename: serbia-company-data-search-api-openapi.yml
  format: yaml
  label: Serbia Company Data Search API
  slug: serbia-company-data-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serbia-company-data/refs/heads/main/openapi/serbia-company-data-search-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vercel.app
  spf: true
hosts:
- cert_expires: Sep 26 13:27:56 2026 GMT
  host: serbia-company-x402.vercel.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Serbia Company Data Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Serbia Company Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Serbia Company Data
provider_slug: serbia-company-data
slug: serbia-company-data-domain-security
source_filename: serbia-company-data-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: serbia-company-x402.vercel.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 13:27:56 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: vercel.app\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/serbia-company-data/refs/heads/main/security/serbia-company-data-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Serbia
- Company Data
- Business Registry
- Open Data
- x402
- base-usdc
- OpenAPI
- Financial Statements
- pay-per-call
- agent-native
---
