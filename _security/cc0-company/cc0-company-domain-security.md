---
api_specs:
- filename: cc0-company-openapi-generated.yml
  format: yaml
  label: CC0 Company API
  slug: cc0-company-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cc0-company/openapi/_ae-authored/cc0-company-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: cc0.company
  spf: true
hosts:
- cert_expires: Dec 12 18:00:10 2026 GMT
  host: cc0.company
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cc0 Company Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CC0 Company, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: CC0 Company
provider_slug: cc0-company
slug: cc0-company-domain-security
source_filename: cc0-company-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cc0.company\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 18:00:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: cc0.company\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/cc0-company/security/cc0-company-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Digital Art
- Social Network
- NFT
- live auctions
- Token Launch
- AI Agents
---
