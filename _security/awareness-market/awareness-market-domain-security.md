---
api_specs:
- filename: awareness-market-openapi-generated.yml
  format: yaml
  label: Awareness API
  slug: awareness-market-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/awareness-market/openapi/_ae-authored/awareness-market-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: awareness.market
  spf: true
hosts:
- cert_expires: Jan  5 15:21:39 2027 GMT
  host: awareness.market
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Awareness Market Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Awareness, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Awareness
provider_slug: awareness-market
slug: awareness-market-domain-security
source_filename: awareness-market-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: awareness.market\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 15:21:39 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: awareness.market\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/awareness-market/security/awareness-market-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Memory
- Agents
- Open Source
- Cloud
---
