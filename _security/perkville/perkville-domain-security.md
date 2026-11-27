---
api_specs:
- filename: perkville-openapi-generated.yml
  format: yaml
  label: Perkville API
  slug: perkville-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/perkville/openapi/_ae-authored/perkville-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: perkville.com
  spf: true
hosts:
- cert_expires: Apr 30 23:59:59 2027 GMT
  host: perkville.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Perkville Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Perkville, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Perkville
provider_slug: perkville
slug: perkville-domain-security
source_filename: perkville-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: perkville.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 30 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: perkville.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/perkville/security/perkville-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Loyalty
- Software-as-a-Service
- Customer Engagement
- Referral Program
- Marketing
---
