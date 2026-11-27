---
api_specs:
- filename: refract-social-openapi-generated.yml
  format: yaml
  label: Refract API
  slug: refract-social-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/refract-social/openapi/_ae-authored/refract-social-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: refract.social
  spf: true
hosts:
- cert_expires: Jan 13 07:28:24 2027 GMT
  host: refract.social
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Refract Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Refract, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Refract
provider_slug: refract-social
slug: refract-social-domain-security
source_filename: refract-social-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: refract.social\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 07:28:24 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: refract.social\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/refract-social/security/refract-social-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Social Media
- Scheduling
- Artificial Intelligence
- Automation
- Company
---
