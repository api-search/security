---
api_specs:
- filename: freeqrly-com-openapi-generated.yml
  format: yaml
  label: FreeQrly API
  slug: freeqrly-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/freeqrly-com/openapi/_ae-authored/freeqrly-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: freeqrly.com
  spf: true
hosts:
- cert_expires: Jan 11 12:18:00 2027 GMT
  host: freeqrly.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: FreeQrly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FreeQrly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: FreeQrly
provider_slug: freeqrly-com
slug: freeqrly-com-domain-security
source_filename: freeqrly-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: freeqrly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 12:18:00 2027 GMT\n  hsts: false\ndomains:\n- domain: freeqrly.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/freeqrly-com/security/freeqrly-com-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- QR Codes
- Privacy
- Static Generation
---
