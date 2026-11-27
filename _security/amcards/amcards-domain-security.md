---
api_specs:
- filename: amcards-openapi-generated.yml
  format: yaml
  label: AMcards API
  slug: amcards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amcards/openapi/_ae-authored/amcards-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: amcards.com
  spf: false
hosts:
- cert_expires: Jan  8 01:54:53 2027 GMT
  host: amcards.com
  hsts: true
  hsts_max_age: 60
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: AMcards Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AMcards, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: AMcards
provider_slug: amcards
slug: amcards-domain-security
source_filename: amcards-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: amcards.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 01:54:53 2027 GMT\n  hsts: true\n  hsts_max_age: 60\ndomains:\n- domain: amcards.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/amcards/security/amcards-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Appreciation-Marketing
- Cards
- Customer Engagement
- Software-as-a-Service
- Marketing
---
