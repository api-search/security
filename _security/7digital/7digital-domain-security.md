---
api_specs:
- filename: 7digital-api-openapi.yml
  format: yaml
  label: 7digital API
  slug: 7digital-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/7digital/refs/heads/main/openapi/7digital-api-openapi.yml
- filename: 7digital-streaming-platform-openapi.yml
  format: yaml
  label: MassiveMusic Streaming Platform API
  slug: massivemusic-streaming-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/7digital/refs/heads/main/openapi/7digital-streaming-platform-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: 7digital.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: massivemusic.com
  spf: true
hosts:
- cert_expires: Jan  9 12:16:51 2027 GMT
  host: uk.7digital.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 21:02:48 2026 GMT
  host: docs.massivemusic.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  9 12:16:51 2027 GMT
  host: api.7digital.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 7Digital Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 7digital, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: 7digital
provider_slug: 7digital
slug: 7digital-domain-security
source_filename: 7digital-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: uk.7digital.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 12:16:51 2027 GMT\n  hsts: false\n- host: docs.massivemusic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 21:02:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.7digital.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 12:16:51 2027 GMT\n  hsts: false\ndomains:\n- domain: 7digital.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: massivemusic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/7digital/refs/heads/main/security/7digital-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Music
- Streaming
- Licensing
- Catalogue
- B2B
- Royalty Reporting
- Public APIs
---
