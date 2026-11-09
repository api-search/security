---
api_specs:
- filename: bnm-farm-free-api-openapi.yml
  format: yaml
  label: BNM Data Shop Free API
  slug: bnm-farm-free-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bnm-farm/openapi/bnm-farm-free-api-openapi.yml
- filename: bnm-farm-paid-api-openapi.yml
  format: yaml
  label: BNM Data Shop Paid API
  slug: bnm-farm-paid-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bnm-farm/openapi/bnm-farm-paid-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bnm.farm
  spf: true
hosts:
- cert_expires: Dec 17 20:28:03 2026 GMT
  host: bnm.farm
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bnm Farm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BNM Data Shop, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: BNM Data Shop
provider_slug: bnm-farm
slug: bnm-farm-domain-security
source_filename: bnm-farm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bnm.farm\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 20:28:03 2026 GMT\n  hsts: false\ndomains:\n- domain: bnm.farm\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/bnm-farm/security/bnm-farm-domain-security.yml
summary_line: TLSv1.3
tags:
- Data
- Marketplace
- Compliance
- Agents
---
