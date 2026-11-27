---
api_specs:
- filename: cautellus-com-openapi-generated.yml
  format: yaml
  label: Cautellus API
  slug: cautellus-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cautellus-com/openapi/_ae-authored/cautellus-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: cautellus.com
  spf: true
hosts:
- cert_expires: Jan 31 02:30:16 2027 GMT
  host: cautellus.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cautellus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cautellus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Cautellus
provider_slug: cautellus-com
slug: cautellus-com-domain-security
source_filename: cautellus-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cautellus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 02:30:16 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: cautellus.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/cautellus-com/security/cautellus-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Scam Detection
- Artificial Intelligence
- Cybersecurity
- Consumer Protection
- Chrome Extension
- Company
---
