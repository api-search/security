---
api_specs:
- filename: usetapestry-dev-openapi-generated.yml
  format: yaml
  label: Tapestry API
  slug: usetapestry-dev-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usetapestry-dev/openapi/_ae-authored/usetapestry-dev-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: usetapestry.dev
  spf: true
hosts:
- cert_expires: Jan  8 13:11:20 2027 GMT
  host: www.usetapestry.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Usetapestry Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tapestry, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Tapestry
provider_slug: usetapestry-dev
slug: usetapestry-dev-domain-security
source_filename: usetapestry-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.usetapestry.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 13:11:20 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: usetapestry.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/usetapestry-dev/security/usetapestry-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Social
- Solana
- Protocol
- API
- Developer
---
