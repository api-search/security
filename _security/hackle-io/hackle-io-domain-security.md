---
api_specs:
- filename: hackle-io-openapi-generated.yml
  format: yaml
  label: Hackle API
  slug: hackle-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hackle-io/openapi/_ae-authored/hackle-io-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hackle.io
  spf: true
hosts:
- cert_expires: Apr 10 23:59:59 2027 GMT
  host: hackle.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hackle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hackle, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hackle
provider_slug: hackle-io
slug: hackle-io-domain-security
source_filename: hackle-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hackle.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 10 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: hackle.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/hackle-io/security/hackle-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- A/B Testing
- Feature Management
- Remote Config
- Data Analytics
- CRM Marketing
- Funnel Analysis
---
