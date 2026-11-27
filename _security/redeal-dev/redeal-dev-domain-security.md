---
api_specs:
- filename: redeal-dev-certificates-api-openapi.yml
  format: yaml
  label: Redeal Certificates API
  slug: redeal-dev-certificates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/redeal-dev/openapi/redeal-dev-certificates-api-openapi.yml
- filename: redeal-dev-deals-api-openapi.yml
  format: yaml
  label: Redeal Deals API
  slug: redeal-dev-deals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/redeal-dev/openapi/redeal-dev-deals-api-openapi.yml
- filename: redeal-dev-onboarding-api-openapi.yml
  format: yaml
  label: Redeal Onboarding API
  slug: redeal-dev-onboarding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/redeal-dev/openapi/redeal-dev-onboarding-api-openapi.yml
- filename: redeal-dev-transparency-api-openapi.yml
  format: yaml
  label: Redeal Transparency API
  slug: redeal-dev-transparency-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/redeal-dev/openapi/redeal-dev-transparency-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dns_aid:
    checked: '2026-11-23'
    published: false
  dnssec: false
  domain: redeal.dev
  spf: true
hosts:
- cert_expires: Jan  8 17:18:25 2027 GMT
  host: redeal.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Redeal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Redeal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Redeal
provider_slug: redeal-dev
slug: redeal-dev-domain-security
source_filename: redeal-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: redeal.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 17:18:25 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: redeal.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n  dns_aid:\n    checked: '2026-11-23'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/redeal-dev/security/redeal-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Fairness Computation
- API
- Sealed‑Bid Auction
- Shapley Value
- Verification
---
