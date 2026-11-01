---
api_specs:
- filename: meld-headless-api-openapi.yml
  format: yaml
  label: Meld.io Headless API
  slug: meld-headless-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meld/openapi/meld-headless-api-openapi.yml
- filename: meld-retail-ramp-api-openapi.yml
  format: yaml
  label: Meld.io Retail Ramp API
  slug: meld-retail-ramp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meld/openapi/meld-retail-ramp-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: meld.io
  spf: true
hosts:
- cert_expires: Nov 21 04:32:02 2026 GMT
  host: meld.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Meld Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Meld.io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Meld.io
provider_slug: meld
slug: meld-domain-security
source_filename: meld-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: meld.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 04:32:02 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: meld.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/meld/security/meld-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data Integration
- FinTech
- API Platform
- Stablecoin
- Digital Assets
- Enterprise
---
