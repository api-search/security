---
api_specs:
- filename: studio-ghibli-openapi.yml
  format: yaml
  label: Studio Ghibli API
  slug: studio-ghibli-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/studio-ghibli/refs/heads/main/openapi/studio-ghibli-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vercel.app
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: herokuapp.com
  spf: false
hosts:
- cert_expires: Sep 26 13:27:56 2026 GMT
  host: ghibliapi.vercel.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 29 23:59:59 2027 GMT
  host: ghibliapi.herokuapp.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Studio Ghibli Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Studio Ghibli, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Studio Ghibli
provider_slug: studio-ghibli
slug: studio-ghibli-domain-security
source_filename: studio-ghibli-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ghibliapi.vercel.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 13:27:56 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: ghibliapi.herokuapp.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 29 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: vercel.app\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: herokuapp.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/studio-ghibli/refs/heads/main/security/studio-ghibli-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Anime
- Studio Ghibli
- Films
- Characters
- Locations
- Species
- Vehicles
- Public APIs
- Open Source
- Read-Only
---
