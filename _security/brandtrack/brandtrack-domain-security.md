---
api_specs:
- filename: brandtrack-openapi-original.yml
  format: yaml
  label: Brandtrack API
  slug: brandtrack-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brandtrack/refs/heads/main/openapi/brandtrack-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: brandtrack.fm
  spf: true
hosts:
- cert_expires: Sep 14 05:14:23 2026 GMT
  host: brandtrack.fm
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 21 23:59:59 2026 GMT
  host: api.brandtrack.fm
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Brandtrack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brandtrack, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Brandtrack
provider_slug: brandtrack
slug: brandtrack-domain-security
source_filename: brandtrack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: brandtrack.fm\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 05:14:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.brandtrack.fm\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 21 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: brandtrack.fm\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brandtrack/refs/heads/main/security/brandtrack-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Music
- Background Music
- Audio
- Streaming
- Retail
- Hospitality
- In-Store Experience
- Media
- Sound
---
