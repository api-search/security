---
api_specs:
- filename: amply-tools-openapi-generated.yml
  format: yaml
  label: Amply API
  slug: amply-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amply-tools/openapi/_ae-authored/amply-tools-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: amply.tools
  spf: true
hosts:
- cert_expires: Jan 30 13:27:05 2027 GMT
  host: amply.tools
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Amply Tools Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amply, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Amply
provider_slug: amply-tools
slug: amply-tools-domain-security
source_filename: amply-tools-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: amply.tools\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 13:27:05 2027 GMT\n  hsts: false\ndomains:\n- domain: amply.tools\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/amply-tools/security/amply-tools-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Personalization
- Mobile
- SDK
- In-App
- Analytics
---
