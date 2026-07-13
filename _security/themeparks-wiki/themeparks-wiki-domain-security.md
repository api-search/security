---
api_specs:
- filename: themeparks-wiki-openapi.yml
  format: yaml
  label: ThemeParks.wiki API
  slug: themeparks-wiki
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/themeparks-wiki/refs/heads/main/openapi/themeparks-wiki-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: themeparks.wiki
  spf: true
hosts:
- cert_expires: Sep 14 18:48:04 2026 GMT
  host: themeparks.wiki
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 00:14:15 2026 GMT
  host: api.themeparks.wiki
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Themeparks Wiki Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ThemeParks.wiki, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ThemeParks.wiki
provider_slug: themeparks-wiki
slug: themeparks-wiki-domain-security
source_filename: themeparks-wiki-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: themeparks.wiki\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 18:48:04 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: api.themeparks.wiki\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 00:14:15 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: themeparks.wiki\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/themeparks-wiki/refs/heads/main/security/themeparks-wiki-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Entertainment
- Real-Time
- Theme Parks
- Wait Times
- Travel
---
