---
api_specs:
- filename: genius-openapi.yml
  format: yaml
  label: Genius
  slug: genius
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/genius/refs/heads/main/openapi/genius-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: genius.com
  spf: true
hosts:
- cert_expires: Aug 11 22:14:24 2026 GMT
  host: genius.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 11 22:14:24 2026 GMT
  host: docs.genius.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 11 22:14:24 2026 GMT
  host: api.genius.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Genius Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Genius, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Genius
provider_slug: genius
slug: genius-domain-security
source_filename: genius-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: genius.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 11 22:14:24 2026 GMT\n  hsts: false\n- host: docs.genius.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 11 22:14:24 2026 GMT\n  hsts: false\n- host: api.genius.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 11 22:14:24 2026 GMT\n  hsts: null\ndomains:\n- domain: genius.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/genius/refs/heads/main/security/genius-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Music
- Lyrics
- Annotations
- Crowdsourced
- Reference Data
- Public APIs
---
