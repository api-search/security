---
api_specs:
- filename: leadsmarts-app-openapi-generated.yml
  format: yaml
  label: LeadSmarts API
  slug: leadsmarts-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leadsmarts-app/openapi/_ae-authored/leadsmarts-app-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: leadsmarts.app
  spf: false
hosts:
- cert_expires: Feb  1 14:13:53 2027 GMT
  host: leadsmarts.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: LeadSmarts Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LeadSmarts, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: LeadSmarts
provider_slug: leadsmarts-app
slug: leadsmarts-app-domain-security
source_filename: leadsmarts-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: leadsmarts.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 14:13:53 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: leadsmarts.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/leadsmarts-app/security/leadsmarts-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Lead Qualification
- Artificial Intelligence
- Sales Enablement
- B2B SaaS
- Privacy
---
