---
api_specs:
- filename: antimatter-openapi-generated.yml
  format: yaml
  label: Antimatter API
  slug: antimatter-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antimatter/openapi/_ae-authored/antimatter-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: antimatter.io
  spf: true
hosts:
- cert_expires: Dec 27 02:53:12 2026 GMT
  host: www.antimatter.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Antimatter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Antimatter, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Antimatter
provider_slug: antimatter
slug: antimatter-domain-security
source_filename: antimatter-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.antimatter.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 02:53:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: antimatter.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/antimatter/security/antimatter-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data Platform
- Analytics
- AI
- Machine Learning
---
