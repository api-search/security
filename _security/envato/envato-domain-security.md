---
api_specs:
- filename: envato-market-api-openapi.yml
  format: yaml
  label: Envato Market API
  slug: envato-market-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/envato/refs/heads/main/openapi/envato-market-api-openapi.yml
- filename: envato-search-api-openapi.yml
  format: yaml
  label: Envato Search API
  slug: envato-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/envato/refs/heads/main/openapi/envato-search-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: envato.com
  spf: true
hosts:
- cert_expires: Dec 20 07:23:15 2026 GMT
  host: envato.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 19 16:14:21 2026 GMT
  host: build.envato.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 19 14:32:55 2026 GMT
  host: api.envato.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
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
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: envato.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 07:23:15 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: build.envato.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 16:14:21 2026 GMT\n  hsts: false\n- host: api.envato.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 14:32:55 2026 GMT\n  hsts: null\ndomains:\n- domain: envato.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
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
- Australia
---
