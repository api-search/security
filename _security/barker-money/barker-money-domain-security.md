---
api_specs:
- filename: barker-money-openapi-generated.yml
  format: yaml
  label: Barker Money API
  slug: barker-money-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/barker-money/openapi/_ae-authored/barker-money-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: barker.money
  spf: true
hosts:
- cert_expires: Dec 19 10:46:06 2026 GMT
  host: barker.money
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Barker Money Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Barker Money, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Barker Money
provider_slug: barker-money
slug: barker-money-domain-security
source_filename: barker-money-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: barker.money\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 10:46:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: barker.money\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/barker-money/security/barker-money-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Finance
- Cryptocurrency
- Yield
- DeFi
- AgentEconomy
---
