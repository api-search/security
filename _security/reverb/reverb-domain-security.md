---
api_specs:
- filename: swagger
  format: yaml
  label: Reverb REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://reverb.com/swagger
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: reverb.com
  spf: true
hosts:
- cert_expires: Sep  8 20:02:53 2026 GMT
  host: reverb.com
  hsts: true
  hsts_max_age: 631138519
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Reverb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Reverb, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Reverb
provider_slug: reverb
slug: reverb-domain-security
source_filename: reverb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: reverb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 20:02:53 2026 GMT\n  hsts: true\n  hsts_max_age: 631138519\ndomains:\n- domain: reverb.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reverb/refs/heads/main/security/reverb-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Marketplace
- Music
- Instruments
- Ecommerce
---
