---
api_specs:
- filename: planetscale-platform-api-openapi.yml
  format: yaml
  label: PlanetScale Platform API
  slug: platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/planetscale/refs/heads/main/openapi/planetscale-platform-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: planetscale.com
  spf: true
hosts:
- cert_expires: Aug 30 06:07:37 2026 GMT
  host: api-docs.planetscale.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  1 23:59:59 2026 GMT
  host: api.planetscale.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 17:50:22 2026 GMT
  host: planetscale.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Planetscale Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for planetscale, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: planetscale
provider_slug: planetscale
slug: planetscale-domain-security
source_filename: planetscale-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api-docs.planetscale.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 06:07:37 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.planetscale.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: planetscale.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 17:50:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: planetscale.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/planetscale/refs/heads/main/security/planetscale-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags: []
---
