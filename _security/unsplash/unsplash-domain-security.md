---
api_specs:
- filename: unsplash-openapi.yml
  format: yaml
  label: Unsplash API
  slug: unsplash
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unsplash/refs/heads/main/openapi/unsplash-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: unsplash.com
  spf: true
hosts:
- cert_expires: Jan  9 18:00:13 2027 GMT
  host: unsplash.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 13 02:00:30 2027 GMT
  host: api.unsplash.com
  hsts: true
  hsts_max_age: 31449600
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Unsplash Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Unsplash, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Unsplash
provider_slug: unsplash
slug: unsplash-domain-security
source_filename: unsplash-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: unsplash.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  9 18:00:13 2027 GMT\n  hsts: null\n- host: api.unsplash.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 13 02:00:30 2027 GMT\n  hsts: true\n  hsts_max_age: 31449600\ndomains:\n- domain: unsplash.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unsplash/refs/heads/main/security/unsplash-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Photos
- Images
- Photography
- Stock Photos
- Creative
- Open Source
- Media
---
