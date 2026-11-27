---
api_specs:
- filename: tareno-co-openapi-generated.yml
  format: yaml
  label: Tareno API
  slug: tareno-co-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tareno-co/openapi/_ae-authored/tareno-co-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dns_aid:
    checked: '2026-11-26'
    published: false
  dnssec: false
  domain: tareno.co
  spf: true
hosts:
- cert_expires: Jan 17 07:18:52 2027 GMT
  host: tareno.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tareno Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tareno, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tareno
provider_slug: tareno-co
slug: tareno-co-domain-security
source_filename: tareno-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tareno.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 07:18:52 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: tareno.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  dns_aid:\n    checked: '2026-11-26'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/tareno-co/security/tareno-co-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Social Media
- Automation
- Content Management
- SaaS
---
