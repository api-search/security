---
api_specs:
- filename: api.json
  format: json
  label: Vocenya API
  slug: vocenya-api
  spec_type: OpenAPI
  url: https://vocenya.com/docs/api.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: vocenya.com
  spf: true
hosts:
- cert_expires: Apr 21 23:59:59 2027 GMT
  host: vocenya.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Vocenya Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for vocenya-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: vocenya-com
provider_slug: vocenya-com
slug: vocenya-com-domain-security
source_filename: vocenya-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vocenya.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 21 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: vocenya.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/vocenya-com/security/vocenya-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI
- Communication
- CustomerService
- Automation
- Voice
---
