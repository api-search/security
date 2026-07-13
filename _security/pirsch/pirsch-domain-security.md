---
api_specs:
- filename: pirsch-pirsch-api-openapi.yml
  format: yaml
  label: Pirsch API
  slug: pirsch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pirsch/refs/heads/main/openapi/pirsch-pirsch-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pirsch.io
  spf: true
hosts:
- cert_expires: Sep 22 05:21:59 2026 GMT
  host: pirsch.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 02:52:28 2026 GMT
  host: docs.pirsch.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 03:11:56 2026 GMT
  host: api.pirsch.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pirsch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pirsch, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Pirsch
provider_slug: pirsch
slug: pirsch-domain-security
source_filename: pirsch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pirsch.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 05:21:59 2026 GMT\n  hsts: false\n- host: docs.pirsch.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 02:52:28 2026 GMT\n  hsts: false\n- host: api.pirsch.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 03:11:56 2026 GMT\n  hsts: null\ndomains:\n- domain: pirsch.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pirsch/refs/heads/main/security/pirsch-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Analytics
- Web Analytics
- Privacy
- GDPR
- Cookie-Free
- Page Views
- Sessions
- Events
- Conversion Goals
- Funnels
- Traffic Sources
---
