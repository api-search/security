---
api_specs:
- filename: lokalise-openapi.yml
  format: yaml
  label: Lokalise API v2
  slug: api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lokalise/refs/heads/main/openapi/lokalise-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lokalise.com
  spf: true
hosts:
- cert_expires: Sep 13 23:59:59 2026 GMT
  host: lokalise.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 15:46:51 2026 GMT
  host: developers.lokalise.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 23:59:59 2026 GMT
  host: api.lokalise.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lokalise Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lokalise, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Lokalise
provider_slug: lokalise
slug: lokalise-domain-security
source_filename: lokalise-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lokalise.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.lokalise.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 15:46:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.lokalise.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lokalise.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lokalise/refs/heads/main/security/lokalise-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Localization
- Translation
- TMS
- AI Machine Translation
- REST
- Developer Tools
---
