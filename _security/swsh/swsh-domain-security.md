---
api_specs:
- filename: swsh-album-api-openapi.yml
  format: yaml
  label: swsh Album API
  slug: swsh-album-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swsh/openapi/swsh-album-api-openapi.yml
- filename: swsh-ping-api-openapi.yml
  format: yaml
  label: swsh Ping API
  slug: swsh-ping-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swsh/openapi/swsh-ping-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: joinswsh.com
  spf: true
hosts:
- cert_expires: Dec 16 20:08:22 2026 GMT
  host: docs.joinswsh.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 22 23:59:59 2027 GMT
  host: public-api.joinswsh.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Swsh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for swsh, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: swsh
provider_slug: swsh
slug: swsh-domain-security
source_filename: swsh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.joinswsh.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 20:08:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: public-api.joinswsh.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 22 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: joinswsh.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/swsh/security/swsh-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fan Engagement
- Live Events
- Photo Sharing
- Software-as-a-Service
---
