---
api_specs:
- filename: unique-domains-openapi-generated.yml
  format: yaml
  label: Unique Domains API
  slug: unique-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/unique-domains/openapi/_ae-authored/unique-domains-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: unique.domains
  spf: true
hosts:
- cert_expires: Jan  2 15:48:21 2027 GMT
  host: unique.domains
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Unique Domains Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Unique Domains, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Unique Domains
provider_slug: unique-domains
slug: unique-domains-domain-security
source_filename: unique-domains-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: unique.domains\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 15:48:21 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: unique.domains\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/unique-domains/security/unique-domains-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Domain
- Data
- Pricing
- Search
---
