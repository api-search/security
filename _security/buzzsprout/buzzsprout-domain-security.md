---
api_specs:
- filename: buzzsprout-openapi.yml
  format: yaml
  label: Buzzsprout Episodes API
  slug: buzzsprout-episodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buzzsprout/refs/heads/main/openapi/buzzsprout-openapi.yml
- filename: buzzsprout-openapi.yml
  format: yaml
  label: Buzzsprout Podcasts API
  slug: buzzsprout-podcasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/buzzsprout/refs/heads/main/openapi/buzzsprout-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: buzzsprout.com
  spf: true
hosts:
- cert_expires: Aug 13 00:48:38 2026 GMT
  host: www.buzzsprout.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Buzzsprout Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Buzzsprout, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Buzzsprout
provider_slug: buzzsprout
slug: buzzsprout-domain-security
source_filename: buzzsprout-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.buzzsprout.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 00:48:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: buzzsprout.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/buzzsprout/refs/heads/main/security/buzzsprout-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Podcasting
- Podcast Hosting
- Audio
- Media
- Episodes
- RSS
---
