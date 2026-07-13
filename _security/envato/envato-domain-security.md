---
api_specs:
- filename: envato-openapi.yml
  format: yaml
  label: Envato Market API
  slug: market
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/envato/refs/heads/main/openapi/envato-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: envato.com
  spf: true
hosts:
- cert_expires: Aug 24 03:27:01 2026 GMT
  host: envato.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 14:32:05 2026 GMT
  host: build.envato.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 13:04:55 2026 GMT
  host: api.envato.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Envato Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Envato, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Envato
provider_slug: envato
slug: envato-domain-security
source_filename: envato-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: envato.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 03:27:01 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: build.envato.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 14:32:05 2026 GMT\n  hsts: false\n- host: api.envato.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 13:04:55 2026 GMT\n  hsts: null\ndomains:\n- domain: envato.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/envato/refs/heads/main/security/envato-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Stock Media
- Marketplace
- Themes
- Audio
- Video
- Graphics
- Subscription
---
