---
api_specs:
- filename: brujula-day-openapi-generated.yml
  format: yaml
  label: Brújula API
  slug: brujula-day-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brujula-day/openapi/_ae-authored/brujula-day-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: brujula.day
  spf: true
hosts:
- cert_expires: Jan 20 01:25:46 2027 GMT
  host: brujula.day
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Brujula Day Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brújula, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Brújula
provider_slug: brujula-day
slug: brujula-day-domain-security
source_filename: brujula-day-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: brujula.day\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 01:25:46 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: brujula.day\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/brujula-day/security/brujula-day-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Productivity
- Organization
- Lifestyle
- Spanish
- Mobile
---
