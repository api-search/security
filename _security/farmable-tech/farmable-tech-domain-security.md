---
api_specs:
- filename: farmable-tech-openapi-generated.yml
  format: yaml
  label: Farmable API
  slug: farmable-tech-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/farmable-tech/openapi/_ae-authored/farmable-tech-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: farmable.tech
  spf: true
hosts:
- cert_expires: Dec 26 16:48:54 2026 GMT
  host: farmable.tech
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Farmable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Farmable, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Farmable
provider_slug: farmable-tech
slug: farmable-tech-domain-security
source_filename: farmable-tech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: farmable.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 16:48:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: farmable.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/farmable-tech/security/farmable-tech-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Agriculture
- Farm Management
- Software-as-a-Service
- Artificial Intelligence
---
