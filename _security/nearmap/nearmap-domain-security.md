---
api_specs:
- filename: nearmap-openapi-generated.yml
  format: yaml
  label: Nearmap API
  slug: nearmap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nearmap/refs/heads/main/openapi/_ae-authored/nearmap-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nearmap.com
  spf: true
hosts:
- cert_expires: Nov 12 08:35:07 2026 GMT
  host: www.nearmap.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Nearmap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nearmap, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Nearmap
provider_slug: nearmap
slug: nearmap-domain-security
source_filename: nearmap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nearmap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 08:35:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: nearmap.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nearmap/refs/heads/main/security/nearmap-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AerialImagery
- Geospatial
- PropertyIntelligence
- APIs
---
