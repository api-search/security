---
api_specs:
- filename: umami-openapi.yml
  format: yaml
  label: Umami API
  slug: umami-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/umami/refs/heads/main/openapi/umami-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: umami.is
  spf: true
hosts:
- cert_expires: Sep 20 01:43:55 2026 GMT
  host: umami.is
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 12 06:35:28 2026 GMT
  host: api.umami.is
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Umami Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Umami, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Umami
provider_slug: umami
slug: umami-domain-security
source_filename: umami-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: umami.is\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 01:43:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.umami.is\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 06:35:28 2026 GMT\n  hsts: null\ndomains:\n- domain: umami.is\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/umami/refs/heads/main/security/umami-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cookieless Tracking
- Open Source
- Privacy
- Web Analytics
- Website Analytics
---
