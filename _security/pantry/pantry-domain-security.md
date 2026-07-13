---
api_specs:
- filename: pantry-openapi.yml
  format: yaml
  label: Pantry API
  slug: pantry
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pantry/refs/heads/main/openapi/pantry-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getpantry.cloud
  spf: false
hosts:
- cert_expires: Aug 21 16:10:45 2026 GMT
  host: getpantry.cloud
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pantry Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pantry, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Pantry
provider_slug: pantry
slug: pantry-domain-security
source_filename: pantry-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getpantry.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 16:10:45 2026 GMT\n  hsts: false\ndomains:\n- domain: getpantry.cloud\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pantry/refs/heads/main/security/pantry-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Data Storage
- Developer Tools
- JSON
---
