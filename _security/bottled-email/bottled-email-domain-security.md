---
api_specs:
- filename: bottled-email-openapi-generated.yml
  format: yaml
  label: Bottled API
  slug: bottled-email-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bottled-email/openapi/_ae-authored/bottled-email-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bottled.email
  spf: true
hosts:
- cert_expires: Dec 23 16:58:38 2026 GMT
  host: bottled.email
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bottled Email Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bottled, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bottled
provider_slug: bottled-email
slug: bottled-email-domain-security
source_filename: bottled-email-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bottled.email\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 16:58:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: bottled.email\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/bottled-email/security/bottled-email-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Email
- Software-as-a-Service
- Cloud
- Productivity
- CustomDomain
---
