---
api_specs:
- filename: inclusifyapp-com-openapi-generated.yml
  format: yaml
  label: Inclusify API
  slug: inclusifyapp-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inclusifyapp-com/openapi/_ae-authored/inclusifyapp-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: inclusifyapp.com
  spf: true
hosts:
- cert_expires: Jan 16 19:12:13 2027 GMT
  host: inclusifyapp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Inclusify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Inclusify, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Inclusify
provider_slug: inclusifyapp-com
slug: inclusifyapp-com-domain-security
source_filename: inclusifyapp-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: inclusifyapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 19:12:13 2027 GMT\n  hsts: false\ndomains:\n- domain: inclusifyapp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/inclusifyapp-com/security/inclusifyapp-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Accessibility
- Web
- Compliance
- Software-as-a-Service
- WCAG
---
