---
api_specs:
- filename: iw-pe-around-api-openapi.yml
  format: yaml
  label: WIPE Around API
  slug: iw-pe-around-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/iw-pe/openapi/iw-pe-around-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: iw.pe
  spf: true
hosts:
- cert_expires: Dec 18 15:54:56 2026 GMT
  host: iw.pe
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: WIPE Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WIPE, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: WIPE
provider_slug: iw-pe
slug: iw-pe-domain-security
source_filename: iw-pe-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: iw.pe\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 15:54:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: iw.pe\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/iw-pe/security/iw-pe-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Website Builder
- BusinessTools
- Multi-language
- PrivacyFocused
---
